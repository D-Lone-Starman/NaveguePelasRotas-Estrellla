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
