# INRUSH Patins e Skates — site da loja

Site da loja **INRUSH Patins e Skates**, em Belém-PA, em **um único arquivo** (`index.html`): HTML, CSS, JavaScript e as fotos, tudo junto. Não precisa instalar nada.

Tem catálogo por categorias, busca, página de cada produto, carrinho que monta o pedido e envia pelo WhatsApp, e a localização da loja.

## Arquivos

```
index.html   o site inteiro
README.md    este guia
```

## Ver no computador

Abra o `index.html` com dois cliques, em um navegador comum (Chrome, Firefox, Safari ou Edge).

## Publicar no GitHub Pages

1. No GitHub, clique em **New repository**, dê um nome (por exemplo `inrush-site`) e crie.
2. Clique em **Add file → Upload files**, arraste o `index.html` e o `README.md` e confirme com **Commit changes**.
3. Vá em **Settings → Pages**, em *Build and deployment* escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
4. Em alguns minutos o site abre em `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.
   Para usar um domínio próprio (por exemplo `inrush.com.br`), preencha **Custom domain** na mesma tela e aponte o DNS conforme as instruções do GitHub.

## Como editar

Abra o `index.html` em um editor de texto e use a busca (Ctrl+F):

- **WhatsApp dos pedidos:** procure `const STORE`. O número vai no formato `55` + DDD + número.
- **Categorias e subcategorias:** procure `const CATEGORIAS`.
- **Produtos:** procure `REAIS.push`. Cada produto tem `nome`, `desc`, `preco` (número em reais, ou `null` para "Consulte o preço"), `cat`, `sub` e `img`.
- **O que fica escondido:** `MOSTRAR_SEM_FOTO`, `ESCONDER_SUBCATEGORIAS_VAZIAS` e `ESCONDER_CATEGORIAS_VAZIAS`. Produto sem foto, subcategoria vazia e categoria vazia não aparecem.
- **Endereço, horários e telefone:** aparecem na página de contato, no rodapé e nos dados para o Google. Procure o número ou a rua para achar todos.

Neste formato as fotos estão embutidas no arquivo, em texto codificado (`data:image/webp;base64,...`). Por isso trocar ou incluir uma foto é trabalhoso. Para manter o catálogo com frequência, o ideal é a versão em pastas (`index.html`, `css/`, `js/`, `images/`), em que as fotos são arquivos soltos e os produtos ficam numa lista própria, `js/produtos.js`.

## Pendências antes de publicar de verdade

- Preços: a maioria dos produtos ainda está "Consulte o preço".
- Fotos: várias fotos vieram de anúncios de outras lojas. Troque por fotos próprias da loja.
- Confirmar com o dono: "12x sem juros", treino aberto toda semana e gratuito, horários e textos das aulas.
- Numeração e tamanhos reais (os tênis estão sem seletor).
- CNPJ, política de troca e devolução e aviso de privacidade no rodapé.
