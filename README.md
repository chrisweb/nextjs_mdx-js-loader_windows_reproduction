#

## reproduction

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser.

![](Error: Only URLs with a scheme in: file, data, and node are supported by the default ESM loader. On Windows, absolute paths must be valid file:// URLs. Received protocol 'c:')

## project setup history

created the project using the CNA command:

`npx create-next-app@canary`

added some dependencies:

`npm i @next/mdx@canary @mdx-js/loader@latest rehype-slug@latest --save-exact`