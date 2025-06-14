# Remlagret.se - Shopify Hydrogen Website

En modern, headless e-handelswebbplats byggd med Shopify Hydrogen för Remlagret.se - Sveriges leverantör av industriella komponenter.

## Funktioner

- 🛍️ Full Shopify-integration
- 🇸🇪 Svenskt språkstöd
- 📱 Responsiv design
- ⚡ Snabb prestanda med Hydrogen
- 🎨 Anpassad design som matchar varumärket

## Teknikstack

- **Framework**: Shopify Hydrogen (Remix)
- **Styling**: Tailwind CSS
- **Språk**: TypeScript
- **E-handel**: Shopify Storefront API
- **Deployment**: Vercel

## Kom igång

1. Klona repositoryt:
\`\`\`bash
git clone https://github.com/Remlagret-se/vercel2.git
cd vercel2
\`\`\`

2. Installera dependencies:
\`\`\`bash
npm install
\`\`\`

3. Sätt upp environment variables:
\`\`\`bash
cp .env.example .env
\`\`\`
Fyll i dina Shopify store-uppgifter i \`.env\`

4. Starta utvecklingsservern:
\`\`\`bash
npm run dev
\`\`\`

## Environment Variables

Nödvändiga environment variables:

- \`PUBLIC_SHOPIFY_STORE_DOMAIN\` - Din Shopify store-domän
- \`PUBLIC_STOREFRONT_API_TOKEN\` - Shopify Storefront API token
- \`PRIVATE_STOREFRONT_API_TOKEN\` - Privat Storefront API token

## Deployment

Detta projekt är konfigurerat för deployment på Vercel:

1. Koppla ditt GitHub-repository till Vercel
2. Sätt environment variables i Vercel dashboard
3. Deploya automatiskt vid push till main branch

## Projektstruktur

\`\`\`
├── app/
│   ├── components/     # Återanvändbara UI-komponenter
│   ├── lib/           # Verktyg och konfigurationer
│   ├── routes/        # Remix routes
│   └── root.tsx       # Root-komponent
├── public/            # Statiska assets
└── ...
\`\`\`

## Licens

Privat - Alla rättigheter förbehållna Remlagret.se
\`\`\`

## 4. Committa README-uppdateringen

```bash type="code"
git add README.md
git commit -m "Update README with correct repository information"
git push origin main
