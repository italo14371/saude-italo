# App de Acompanhamento — Saúde do Ítalo

Página web única (`index.html`) com tudo já pré-configurado: treino atual (academia + corrida + plano B em casa), cardápio base, metas, e um painel de evolução.

## Como usar no celular

**Opção mais simples — abrir o arquivo direto:**
1. Envie o arquivo `index.html` pra você mesmo (WhatsApp, e-mail, AirDrop) e abra no navegador do celular
2. No menu do navegador, use "Adicionar à tela inicial" pra ele ficar com cara de app
3. Os dados ficam salvos no navegador (localStorage) — funciona offline depois de aberto uma vez

**Opção recomendada (mais robusta) — hospedar gratuitamente:**
Posso te ajudar a publicar essa página no **GitHub Pages** (gratuito) — daí você acessa por um link fixo, em qualquer navegador, e dá pra "instalar" como app de verdade (PWA). É um passo opcional, me avise se quiser fazer isso.

## Como funciona

- **Hoje**: registre água (botões rápidos +200/+300/+500ml/+1L), peso do dia, o treino feito (Academia / Corrida / Treino Casa / Descanso) com cargas e reps por série, troca de exercício quando algo está ocupado, refeições do dia (escolha do cardápio ou texto livre) e observações
- **Treino**: referência do plano atual (Treino A, progressão de corrida, Treino Casa)
- **Dieta**: referência do cardápio base e estratégias rápidas
- **Painel**: evolução do peso, água dos últimos 7 dias, progressão de carga por exercício, histórico de corrida, frequência de treino (últimos 14 dias) e badges/streaks

## Backup e revisão com o Claude

Na aba **Painel → Dados**, use "Exportar JSON" de tempos em tempos. Esse arquivo pode ser salvo aqui na pasta (`Treino e dieta/App/backups/`) e, quando quiser, eu reviso sua evolução com base nele e ajusto o plano de treino/dieta.

## Atualizando o plano

Conforme o `treino-coach` e o `nutri-dieta` ajustarem seu treino/cardápio nos arquivos markdown, eu atualizo também o objeto `PLAN` no início do `<script>` do `index.html` pra manter o app sincronizado com o plano oficial.
