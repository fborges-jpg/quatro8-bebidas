# Quatro8 Bebidas — Site V1

Catálogo digital sem preços públicos, com busca completa, navegação por categorias e lista para cotação via WhatsApp.

## Estado da V1
- 699 bebidas da carta TAF
- imagens extraídas e associadas pelo código TAF
- busca por poucas letras, marca/rótulo/país/categoria/tipo/uva/volume/palavras-chave
- Vinhos por país
- Destilados por tipo
- lista para cotação persistida no navegador
- nome + endereço completo antes do WhatsApp
- WhatsApp ainda como placeholder
- sem preços e sem estoque prometido

## Configurar WhatsApp
Editar `public/assets/js/config.js` e preencher `whatsappNumber` apenas com números, incluindo 55 + DDD.

## Seleção da Semana
No mesmo arquivo `config.js`, alterar `selectionOfWeekCodes` com códigos TAF existentes.

## Regras comerciais exibidas
- pedido mínimo: R$ 250 em produtos
- frete R$ 30: Florianópolis e São José
- acima de R$ 1.000: frete grátis
- outras regiões: frete sob consulta
- pagamento: 50% na confirmação + 50% na entrega, via Pix
- entregas: terças e sextas até 20h
- cotação válida por 24 horas
- 18+ / consumo responsável

## Rodar localmente
`python -m http.server 8080 -d public`

## Cloudflare
`npm install`
`npm run dev`
`npm run deploy`

O domínio próprio não é necessário nesta fase; o deploy pode usar o endereço gratuito do projeto.
