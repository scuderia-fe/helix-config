# helix-config
Helix customized configuration: optimized to work with React, Typescript, Tailwind, Eslint and more 💥.

## LSP required for this config
There are the required LSP to make this config work, you'll need to install them globally using your preferred package manager, I use [volta](https://github.com/volta-cli/volta) but you can go with npm if you hate yourself that much.

- [typescript-language-server](https://www.npmjs.com/package/typescript-language-server) - for typescript
- [@tailwindcss/language-server](https://www.npmjs.com/package/@tailwindcss/language-server) - for tailwind
- [vscode-langserver-extracted](https://www.npmjs.com/package/vscode-langservers-extracted) - for emmet, css, html and eslint

You may also need some other packages installed globally, these are not mandatory but if they're not present in your project's `package.json`, things won't work. I prefer to have them installed globally so I don't end up typing `:format` and wait for nothing to happen.
- [typescript](https://www.npmjs.com/package/typescript)
- [prettier](https://www.npmjs.com/package/prettier)
- [tailwindcss](https://www.npmjs.com/package/tailwindcss)

## What this config supports
### Typescript
Typescript is the main focus: we spend the majority of our time working on typescript projects. The goal is to make the LSP-related DX as similar as possible to popular IDES like VsCode or WebStorm.

The configuration for typescript supports the `typescript-language-server` (obviously), `tailwindcss-language-server`, `emmet-language-server` and `eslint-language-server`.
So in `.ts`, `.tsx` and `.jsx` files you get typescript, emmet and tailwind suggestions as well as eslint and typescript errors.

To keep the code clean and organized we use prettier.
