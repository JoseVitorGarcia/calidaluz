# Cálida Luz — Rebuild da Landing Page

**Data:** 2026-06-13  
**Objetivo:** Reconstruir a landing page gerada pelo Google Stitch em um site de conversão real, direcionando visitantes para Shopee e Mercado Livre.

---

## Contexto

A Cálida Luz é uma marca de velas artesanais de soja, com domínio próprio comprado. O site é uma **landing page de conversão** — não há e-commerce próprio; as vendas acontecem via Shopee e Mercado Livre. O conteúdo (fotos, preços, redes sociais) será mockado inicialmente e substituído pelos reais quando disponível.

O ponto de partida é `stitch_c_lida_luz_e_commerce_design/code.html`, gerado pelo Google Stitch, com identidade visual já definida.

---

## Identidade Visual (mantida do Stitch)

- **Paleta:** creme `#fff8f4`, âmbar/primary `#875300`, sage `#586244`, fundo suave `#fff1e6`
- **Tipografia:** Libre Caslon Text (títulos, serif editorial) + DM Sans (corpo, labels)
- **Shapes:** bordas orgânicas, blob-shapes, leaf-shapes — sensação artesanal
- **Tom:** slow living, artesanal, sustentável, aconchegante

---

## Estrutura da Página

### 1. Nav
- Logo "Cálida Luz" (italic, âmbar) à esquerda
- Links: Shop · Essência · Como é Feita · Stories
- Ícone de shopping bag à direita (ancora para #shop, não link direto para marketplace)
- Mobile: menu hamburguer com drawer lateral
- Comportamento: esconde no scroll down, reaparece no scroll up (já implementado no Stitch)

### 2. Hero
- Supertítulo pequeno em sage: "✦ Feito à mão · Pequenos lotes"
- Headline: "Luz que abraça, *calor que transforma.*" (itálico âmbar na segunda linha)
- Subtexto: "Velas artesanais de soja. Para os seus momentos de respiro."
- CTA primário: botão sólido âmbar "Ver coleção →" (ancora para #shop)
- CTA secundário: link texto "Nossa história" (ancora para #essencia)
- Imagem: foto mockada de vela à direita, com border-radius assimétrico
- Background: blob-shape em surface-variant, filter blur

### 3. Barra de Selos de Confiança
- Fundo `surface-container-low`
- 4 selos em linha horizontal: 🌿 Cera 100% Natural · 🐾 Cruelty Free · ✋ Artesanal · 🔥 Queima Limpa
- Cada selo: ícone Material Symbols + label em small-caps DM Sans
- Mobile: grid 2×2

### 4. Produtos — "Aconchego em Chamas"
- Título de seção centralizado
- Grid: 2 colunas em desktop, 1 coluna em mobile
- **Cada card:**
  - Foto (mockada, `object-cover`, border-radius orgânico)
  - Tag "Soja · Vegano" em pill sage no canto da foto
  - Nome do produto (Libre Caslon Text, headline-md)
  - Descrição curta (1-2 linhas, DM Sans, on-surface-variant)
  - Preço em âmbar (22px, bold)
  - Botão sólido âmbar "Shopee" + botão outlined âmbar "Mercado Livre" (lado a lado)
- Hover: scale sutil na foto (já presente no Stitch)
- **Produtos mockados (4):**
  1. Brisa de Lavanda — R$ 49,90
  2. Madeiras Calmas — R$ 54,90
  3. Baunilha & Mel — R$ 44,90
  4. Hortelã Fresca — R$ 47,90

### 5. Nossa Essência
- Layout: imagem circular à esquerda, texto à direita (invertido em mobile: texto em cima)
- Texto sobre a marca: processo artesanal, cera de soja, pavio de algodão, produção em pequenos lotes
- Tags de sustentabilidade (Cera Natural, Cruelty Free, Artesanal) mantidas do Stitch

### 6. Como é Feita — Timeline Artesanal
- Título: "Do início à chama"
- Timeline horizontal em desktop, vertical em mobile
- 5 etapas com ícone + label + descrição curta:
  1. 🧴 Cera de Soja — matéria-prima selecionada
  2. 🌸 Fragrância — blend artesanal de óleos essenciais
  3. 🧵 Pavio — algodão trançado à mão
  4. ⏳ Repouso — 48h para cura e cristalização
  5. 📦 Embalagem — papel reciclado e carinho

### 7. Depoimentos — "Ecos da Luz"
- 3 cards assimétricos mantidos do Stitch (grid bento, rotação sutil)
- Textos mockados das clientes Mariana C., Lucas T. e Sofia R.

### 8. Instagram — "Nos acompanhe"
- Título: "Nos acompanhe" + handle `@calidaluz` em âmbar
- Grid 3×2 de fotos mockadas (tons creme/âmbar, aspecto quadrado)
- Botão "Seguir no Instagram" linkando para `https://instagram.com/calidaluz` (mockado)
- Nota: substituir por embed real quando conta for criada

### 9. Lista de Espera — "Fique por dentro"
- Fundo `surface-container-low`
- Texto: "Receba novidades, lançamentos e promoções em primeira mão."
- Input de email + botão "Quero receber" (âmbar)
- Comportamento: apenas frontend (sem backend); exibe mensagem de confirmação via JS
- Nota: integrar com Mailchimp/Brevo quando disponível

### 10. Rodapé
- Logo Cálida Luz à esquerda
- Links: Sustentabilidade · Contato · Envio
- Links de redes sociais: ícones Instagram, TikTok (mockados)
- Badges textuais: "Disponível na Shopee" + "Disponível no Mercado Livre"
- © 2025 Cálida Luz. Todos os direitos reservados.

---

## Mobile (375px)

- Nav: hamburguer → drawer lateral com links empilhados
- Hero: coluna única, imagem abaixo do texto
- Selos: grid 2×2
- Produtos: 1 coluna, botões Shopee e ML empilhados verticalmente
- Timeline: vertical com linha conectora
- Instagram: grid 3×2 mantido (fotos menores)
- Input de email: largura total

---

## Arquitetura Técnica

- **Stack:** HTML único + Tailwind CDN (mantendo abordagem do Stitch) + vanilla JS
- **Arquivo de saída:** `index.html` na raiz do projeto
- **Imagens:** `https://placehold.co/` para mockups, com `alt` descritivo real
- **Fontes:** Google Fonts (já carregadas no Stitch) — Libre Caslon Text, DM Sans, Material Symbols Outlined
- **Interatividade:**
  - Scroll nav hide/show (já implementado)
  - Hover scale em fotos de produto
  - Menu mobile hamburguer
  - Email capture com feedback visual (JS puro, sem backend)
- **SEO básico:** `<title>`, `<meta description>`, `lang="pt-BR"` (já presente)

---

## Conteúdo Mockado — O que substituir no futuro

| Seção | Mockado agora | Substituir por |
|---|---|---|
| Fotos de produto | placehold.co | Fotos reais das velas |
| Preços | R$ 44–54 | Preços reais |
| Instagram grid | placeholders âmbar | Fotos reais do IG |
| Link Instagram | `#` | URL real da conta |
| Link TikTok | `#` | URL real da conta |
| Email form | apenas frontend | Integração Mailchimp/Brevo |
| Links Shopee/ML | `#` | URLs reais das lojas |

---

## O que NÃO está no escopo

- Carrinho de compras ou checkout próprio
- Sistema de estoque
- Painel administrativo
- Blog
- Múltiplas páginas
