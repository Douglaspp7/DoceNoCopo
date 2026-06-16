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

   - `hero-mujer.jpg`  ← ainda é a foto original do DulceVaso; **substitua pela
     foto da brasileira** quando tiver uma (mantenha esse nome)
   - `app-en-mano.jpg`
   - `demo-app.mp4`
   - `postre-fresa.jpg`, `postre-chocolate.jpg`, `mazamorra-morada.jpg`,
     `fresas-con-chocolate.jpg`, `durazno-con-crema.jpg`, `choco-flan-en-vaso.jpg`
   - `encomiendas.jpg`
   - `mockup-recetas-rentables.png`, `mockup-calculadora.png`, `mockup-plan-ventas.png`,
     `mockup-kit-whatsapp.png`, `mockup-guia-empaque.png`, `mockup-recetas.png`

4. Conecte ao **Cloudflare Pages** (Connect to Git → este repo → build command vazio,
   output dir `/`).

## Antes de anunciar — TROQUE

- **`CHECKOUT_URL`** (topo do `index.html`): coloque o link da oferta **BR de R$ 27,90**
  no Hotmart. O link atual é placeholder (produto em USD).
- **`hero-mujer.jpg`**: troque pela foto com biotipo brasileiro.
- URLs `og:` / `canonical` no `<head>`: ajuste para o seu domínio do Cloudflare.
