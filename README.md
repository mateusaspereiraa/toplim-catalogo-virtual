# Toplim — Catálogo Virtual

Abra `index.html` no navegador (ou publique a pasta em qualquer hospedagem estática).

## Estrutura

```
index.html          estrutura da página
manifest.json       configuração do app instalável (PWA)
css/styles.css      todos os estilos
js/data.js          produtos e lista de fotos (edite aqui para atualizar o catálogo)
js/app.js           lógica: busca, filtros, cards, painel admin, PDF, tema
assets/             logos e ícones
img-produtos/       fotos dos produtos, nomeadas pelo código: <código>.webp
docs/               material de referência (não é usado pelo site; pode apagar)
```

## Como adicionar uma foto
1. Salve a imagem como `img-produtos/<código do produto>.webp`.
2. Inclua o código na lista `IMAGENS_DISPONIVEIS` em `js/data.js`.

O card do produto passa a exibir a foto automaticamente.

## Observações
- Alterações feitas no painel **Administrador** ficam salvas no navegador (localStorage).
  Use *Dados → Exportar JSON* para fazer backup.
- O botão **PDF** abre a impressão do navegador com todos os produtos filtrados; escolha "Salvar como PDF".
