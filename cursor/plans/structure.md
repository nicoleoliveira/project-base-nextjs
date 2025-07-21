# Plano de Estrutura Inicial do Projeto

## 1. Inicialização do Projeto

- Criar um novo projeto Next.js com TypeScript, diretamente no diretório desejado (sem subdiretório).

## 2. Instalação e Configuração do Tailwind CSS

- Instalar as dependências:  
  `npm install tailwindcss @tailwindcss/postcss postcss`
- Criar/editar o arquivo `postcss.config.mjs` com o plugin do Tailwind.
- Importar o Tailwind CSS no arquivo global de estilos (`app/globals.css` ou `src/app/globals.css`).

## 3. Instalação e Configuração do shadcn/ui

- Instalar e inicializar a biblioteca de componentes shadcn/ui.

## 4. Criação da Estrutura de Diretórios para Autenticação

- Criar os diretórios principais para rotas de autenticação e rotas protegidas, seguindo a convenção do Next.js App Router.

## 5. Estrutura Recomendada de Pastas

```
project-base/
│
├── app/
│   ├── layout.tsx
│   ├── page.tsx
│   ├── globals.css
│   ├── (auth)/
│   │   ├── login/page.tsx
│   │   ├── register/page.tsx
│   │   └── forgot-password/page.tsx
│   └── (protected)/
│       └── page.tsx
│
├── components/
├── context/
├── lib/
├── styles/
│
├── public/
├── .env.local
├── postcss.config.mjs
├── tailwind.config.js (opcional, se quiser customizar)
├── next.config.js/ts
└── package.json
```

## 6. Observações

- Não será implementada nenhuma lógica de autenticação, apenas a estrutura de pastas e arquivos principais.
- As rotas de autenticação ficam dentro de `app/(auth)/`.
- As rotas protegidas ficam em `app/(protected)/`.
- Os diretórios `components/`, `context/` e `lib/` são criados para futura expansão e organização do código. 