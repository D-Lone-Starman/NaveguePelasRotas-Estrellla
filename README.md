This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```# NaveguePelasRotas+SeuSobrenome

Este é um projeto de loja virtual desenvolvido com **Next.js + TypeScript + TailwindCSS**, como parte da entrega do curso.

## ✅ Funcionalidades Implementadas

### Rotas
- Utilização do App Router do Next.js (`/app`)
- Rota para **catálogo principal**: `/`
- Rota dinâmica para **categorias de produtos**: `/category/[categoryId]`
- Rota dinâmica para **detalhes de produtos**: `/item/[productId]`
- Rota 404 personalizada (`not-found.tsx`)

### Componentização
- Separação entre:
  - **Componentes de apresentação** (`ProdutoCard`, `Cabecalho`, `Rodape`, etc.)
  - **Componentes containers com lógica de estado** (`page.tsx`, `[categoryId]/page.tsx`, `[productId]/page.tsx`)
- `ListaProdutos` utiliza `.map()` com `key` correta

### Navegabilidade
- Uso de `useParams` para capturar rotas dinâmicas
- Atualização automática ao mudar de categoria ou acessar um produto
- Carrinho funcional com `useState`, permitindo adicionar/remover/editar quantidades

## 📁 Estrutura de Pastas
app/
├── page.tsx # Catálogo principal
├── category/
│ └── [categoryId]/page.tsx # Catálogo por categoria
├── item/
│ └── [productId]/page.tsx # Detalhes do produto
components/
├── Products/
│ ├── ProdutoCard.tsx
│ └── ListaProdutos.tsx
├── Cart/
│ └── Carrinho.tsx
data/
└── produtos.ts # Array simulado de produtos (mock)


## 🔧 Tecnologias utilizadas

- Next.js (App Router)
- React (client components)
- TypeScript
- TailwindCSS
- Hooks (`useState`, `useEffect`, `useParams`)
- Modularização de componentes

## 🚀 Como rodar

1 - Clone o repositório
2 -Instale as dependências:
   bash
   npm install

3- Inicie o servidor:
npm run dev

4- Acesse http://localhost:3000





Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
