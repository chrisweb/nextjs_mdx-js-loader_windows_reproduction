# reproduction repository: next.js mdx js loader bug on windows

First clone this repository, and then install the [dependencies](package.json):

```bash
npm i
```

Then start the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser.

If on windows you should see the following error:

![Error: Only URLs with a scheme in: file, data, and node are supported by the default ESM loader. On Windows, absolute paths must be valid file:// URLs. Received protocol 'c:'](https://raw.githubusercontent.com/chrisweb/nextjs_mdx-js-loader_windows_reproduction/refs/heads/main/public/problem_windows_screenshot.png)

```shell
Error: Only URLs with a scheme in: file, data, and node are supported by the default ESM loader. On Windows, absolute paths must be valid file:// URLs. Received protocol 'c:'
```

## project setup history

created the project using the CNA command:

`npx create-next-app@canary`

added some dependencies:

`npm i @next/mdx@canary @mdx-js/loader@latest rehype-slug@latest --save-exact`