# Amavi Macarons Artesanais (demo)

Landing page de demonstração, HTML único (`index.html`), sem dependências além das fontes do Google Fonts. Não publicada.

## Estrutura
- `index.html`: o site (hero com foto em arco, vitrine em mosaico com ampliação, "Monte a sua caixa", como pedir, contato e bloco final)
- `Copy.txt`: texto da página
- `design-system-amavi.md` / `.html`: design system
- `assets/`: logos, símbolo, favicon, imagem de compartilhamento e `foto-*.jpg`
- `Logo/`: logo original. `Imagens/` e `Fotos/`: referências do Pinterest (não são fotos da Amavi; ignoradas pelo git). **Trocar as `assets/foto-*.jpg` pelas fotos reais antes de publicar.**

## WhatsApp
`WA_NUMBER` está vazio porque o número não foi informado. Sem número, os links abrem `wa.me/?text=...`. Ao receber o número, preencher (DDI+DDD+número, só dígitos).

## Como visualizar
`node "_ferramentas/preview-local.mjs" "4. Meus Clientes/2. Demos e propostas/amavi"` e abrir o endereço mostrado.

## Antes de publicar
- Remover `<meta name="robots" content="noindex, nofollow">`.
- Itens `[A CONFIRMAR]` aparecem com borda tracejada; lista na ficha `_Fichas/Amavi.pdf`.
- Confirmar sabores, tamanhos, valores, cidade, entrega, WhatsApp, Instagram e história.
- Usar endereço absoluto em `og:image` quando houver domínio; pedir a logo em alta resolução.
