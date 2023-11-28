# eslint-config
//comandos para inicializacao
npm install eslint --save-dev
yarn add eslint-plugin-import-helpers eslint-import-resolver-typescript -D
yarn add prettier eslint-config-prettier eslint-plugin-prettier -D

configuracoes do eslint.json
{
    "env": {
        "browser": true,
        "es2021": true
    },
    "extends": [
        "standard-with-typescript",
        "plugin:react/recommended",
        "plugin:@typescript-eslint/recommended",
        "prettier",
        "plugin:prettier/recommended"
    ],
    "parser": "@typescript-eslint/parser",
    "parserOptions": {
        "ecmaFeatures": {
            "jsx": true
        },
        "ecmaVersion": "latest",
        "sourceType": "module"
    },
    "plugins": [
        "react",
        "@typescript-eslint",
        "eslint-plugin-import-helpers",
        "prettier",
    ],
    "rules": {
        "@typescript-eslint/explicit-function-return-type": "off"
    }
}
