# doce-no-copo

Landing page (pt-BR) do **DulceVaso** adaptada para o mercado **brasileiro**.

- Idioma: Português do Brasil
- Oferta: **R$ 27,90** (pagamento único)
- Público/checkout: **somente Brasil** (PIX, boleto, cartão via Hotmart)
- Pixel: mesmo Meta Pixel do projeto principal

## Como publicar

1. Crie este repositório no GitHub: `doce-no-copo`.
2. `index.html` já está pronto na raiz.
3. Os **arquivos de mídia** abaixo já foram copiados do repositório DulceVaso e
   estão na raiz, ao lado do `index.html`:

   - `hero-mujer.jpg`  ← já é a foto brasileira
   - `app-en-mano.jpg`
   - `demo-app.mp4`
   - `postre-fresa.jpg`, `postre-chocolate.jpg`, `mazamorra-morada.jpg`,
     `fresas-con-chocolate.jpg`, `durazno-con-crema.jpg`, `choco-flan-en-vaso.jpg`
   - `encomiendas.jpg`
   - `mockup-recetas-rentables.png`, `mockup-calculadora.png`, `mockup-plan-ventas.png`,
     `mockup-kit-whatsapp.png`, `mockup-guia-empaque.png`, `mockup-recetas.png`

4. Conecte ao **Cloudflare Pages** (Connect to Git → repo `Douglaspp7/DoceNoCopo` →
   production branch `main` → build command vazio → output dir `/`).
   Nomeie o projeto **`doce-no-copo`** para que a URL gerada seja
   `doce-no-copo.pages.dev` (já configurado nas tags `og:`/`canonical`).

## Antes de anunciar — TROQUE

- **`CHECKOUT_URL`** (topo do `index.html`): ainda é o placeholder em USD do
  DulceVaso. Troque pelo link da oferta **BR de R$ 27,90** no Hotmart antes
  de divulgar.
- Se usar um domínio próprio em vez de `doce-no-copo.pages.dev`, atualize as
  URLs `og:url`, `og:image` e `canonical` no `<head>` do `index.html`.

## Mockups ainda em espanhol — TROQUE

Estas imagens vieram do DulceVaso e ainda têm texto em espanhol. Use
`Order Pump/gerador-mockups-pt-br.html` (abra localmente no navegador, cole
sua chave de API da OpenAI ou do Gemini) para gerar as versões em português
e baixe substituindo os arquivos com o **mesmo nome** na raiz do repo:

- [ ] `app-en-mano.jpg`
- [ ] `mockup-recetas-rentables.png`
- [ ] `mockup-calculadora.png`
- [ ] `mockup-plan-ventas.png`
- [ ] `mockup-kit-whatsapp.png`
- [ ] `mockup-guia-empaque.png`
- [ ] `mockup-recetas.png`
- [ ] `encomiendas.jpg` (opcional — só os nomes nas etiquetas, não é bem espanhol)

`hero-mujer.jpg` e as 6 fotos da galeria de receitas (`postre-fresa.jpg` etc.)
não têm texto na imagem, então não precisam de troca.

Os nomes de arquivo e os `alt=""` no `index.html` já estão em português —
basta substituir o conteúdo de cada imagem, sem editar HTML.
