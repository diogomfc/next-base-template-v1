npx create-next-app project-name -e https://github.com/diogomfc/next-base-template-v1

```bash
   INSTALL ESLINT
   npx eslint --init
```

```bash
  INSTALL PRETTIER
  Prettier - https://prettier.io/docs/en/install.html
  
   pnpm install --save-dev --save-exact prettier

   create .prettierrc.json in root directory
    add in .prettierrc.json
      {
      "traillingComma": "none",
      "semi": true,
      "singleQuote": true
      }
```

```bash
  INSTALL PLUGIN
  ---
  eslint-plugin-react-hooks - https://github.com/facebook/react/tree/main/packages/eslint-plugin-react-hooks
  pnpm install eslint-plugin-react-hooks --save-dev
  
  add in .eslintrc.json

  {
  "plugins": [
    // ...
    "react-hooks"
  ],
  "rules": {
    // ...
    "react-hooks/rules-of-hooks": "error",
    "react-hooks/exhaustive-deps": "warn"
  }
  }
  ----
  eslint-config-prettier - https://github.com/prettier/eslint-config-prettier#installation
  pnpm install --save-dev eslint-config-prettier

  add in .eslintrc.json

  {
  "extends": [
    "prettier"
  ]
  }

  ----
  eslint-plugin-prettier - https://github.com/prettier/eslint-plugin-prettier
  pnpm install --save-dev eslint-plugin-prettier

  add in .eslintrc.json

  {
    "rules": {
    "prettier/prettier": "error"
     }
  }

  ----
  eslint-plugin-import-helpers - https://github.com/Tibfib/eslint-plugin-import-helpers/tree/master
  pnpm install eslint-plugin-import-helpers --save-dev

  add in .eslintrc.json

    plugins: ['eslint-plugin-import-helpers'],
    rules: {
        'import-helpers/order-imports': [
            'warn',
            { // example configuration
                newlinesBetween: 'always',
                groups: [
                    'module',
                    '/^@shared/',
                    ['parent', 'sibling', 'index'],
                ],
                alphabetize: { order: 'asc', ignoreCase: true },
            },
        ],
    }
}

```
