# Design system: Amavi Macarons Artesanais

Direção definida em 09/10/2026, depois de o usuário reprovar duas versões (a primeira apagada e a segunda poluída): **foto grande e limpo**, como uma doceria premium. A foto é a protagonista, a paleta é curta e o espaço em branco faz o trabalho.

## Tom visual (3 linhas)
1. Fundo branco-quente e rosa-bebê, texto vinho, um único acento framboesa para ação.
2. Fotos grandes, em arco e em cantos arredondados; nada de desenho, faixa ou borda decorativa.
3. Tipografia serifada leve (Fraunces) com itálico no acento, sans fina (Outfit) no corpo e muito espaço.

## 1. Cores

| Papel | Token | Hex | Uso |
|---|---|---|---|
| Fundo | --bg | #FFFBF8 | Fundo padrão |
| Rosa-bebê | --blush | #FCEFEC | Seções alternadas |
| Rosa 2 | --blush2 | #F6DAD6 | Halo do hero e fundo de foto carregando |
| Tinta | --ink | #2B1814 | Texto, botão secundário, rodapé |
| Texto secundário | --muted | #6F5A55 | Apoio |
| Marca (logo) | --brand | #7A3320 | Nome "Amavi" no topo (cor da logo) |
| Framboesa | --acc | #B3123F | Botão principal, itálicos, números |
| Framboesa escuro | --acc-d | #8F0E31 | Hover do botão principal |
| Linha | --line | #EFDDD8 | Bordas finas |
| WhatsApp | --wa | #25D366 | **Exclusivo** do botão e do flutuante (texto escuro) |

Regras: o verde do WhatsApp nunca é decorativo. O framboesa é o único acento.

## 2. Tipografia

| Uso | Fonte | Peso |
|---|---|---|
| Títulos | Fraunces (normal e itálico) | 300 nos grandes, 400 nos pequenos |
| Corpo e rótulos | Outfit | 300, 400 e 500 |

## 3. Componentes
- **Botão principal:** framboesa com texto branco, pílula. **Secundário:** contorno tinta. **WhatsApp:** verde com texto escuro.
- **Foto em arco:** topo semicircular, base arredondada, sombra suave rosada.
- **Mosaico da vitrine:** 7 fotos em 12 colunas, legenda sobre a foto, ampliação ao toque; no celular vira 2 colunas.
- **Linha de sabor:** bolinha de cor, nome serifado, botões − e + de 44 px.
- **Cartão "Sua caixa":** barra de progresso, lista dos sabores e botão de WhatsApp; fixo ao lado no desktop.
- **Pendência:** borda tracejada com "[A CONFIRMAR]", sempre visível.

## 4. Estética e movimento
Raios de 28 px nas fotos e cartões, 999 px em botões e chips. Sombras suaves em rosado. Movimento mínimo (entrada do hero, revelação ao rolar com plano B, hover nas fotos), tudo desligado com `prefers-reduced-motion`.

## 5. Conversão
"Monte a sua caixa" monta o pedido (tamanho, sabores, ocasião, data, nome e recado) e abre o WhatsApp com tudo escrito. Botão flutuante sempre à mão. Sem preço, prazo ou promessa.

## Tokens (CSS)
```css
:root{
  --bg:#FFFBF8; --blush:#FCEFEC; --blush2:#F6DAD6; --ink:#2B1814; --muted:#6F5A55; --brand:#7A3320;
  --acc:#B3123F; --acc-d:#8F0E31; --line:#EFDDD8; --wa:#25D366;
  --serif:'Fraunces',Georgia,serif; --sans:'Outfit',sans-serif; --r:28px;
}
```
