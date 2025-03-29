# chonos-pomodoro

Este projeto utiliza React + TypeScript + Vite, com configuração mínima e suporte a HMR e ESLint.

---

## Configuração padrão do Vite

Este template fornece uma base para começar com:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) usando [Babel](https://babeljs.io/) para Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) usando [SWC](https://swc.rs/) para Fast Refresh

### Expansão da configuração do ESLint

Se estiver desenvolvendo uma aplicação para produção, recomendamos habilitar regras com verificação de tipo:

```js
export default tseslint.config({
  extends: [
    ...tseslint.configs.recommendedTypeChecked,
    ...tseslint.configs.strictTypeChecked,
    ...tseslint.configs.stylisticTypeChecked,
  ],
  languageOptions: {
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})