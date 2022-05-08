### Start the project

    yarn init -y

### Create file .editorconfig with the content:

    # EditorConfig is awesome: https://EditorConfig.org

    # top-most EditorConfig file
    root = true

    # Unix-style newlines with a newline ending every file
    [*]
    indent_style = space
    indent_size = 4
    end_of_line = crlf
    charset = utf-8
    trim_trailing_whitespace = false
    insert_final_newline = false

### Install typescript with dependency of development, run:

    yarn add -D typescript

    yarn tsc --init

### Content for file tsconfig.json:

    {
        "compilerOptions": {
            "target": "es2020",
            "module": "commonjs",
            "allowJs": true,
            "esModuleInterop": true,
            "forceConsistentCasingInFileNames": true,
            "skipLibCheck": true,
            "outDir": "./dist"
        }
    }

### Add Eslint, run and answer the questions:

    yarn add -D eslint
    yarn eslint --init

### Config eslint and prettier, run:

    yarn add prettier eslint-config-prettier eslint-plugin-prettier babel-eslint -D

### cofigure eslint, put the content on .eslintrc.json:

    {
        "env": {
            "es2021": true,
            "node": true
        },
        "extends": [
            "standard", "prettier"
        ],
        "parser": "@typescript-eslint/parser",
        "parserOptions": {
            "ecmaVersion": "latest",
            "sourceType": "module"
        },
        "plugins": [
            "@typescript-eslint", "prettier"
        ],
        "rules": {
            "prettier/prettier": "error"
        }
    }

### Add ts-node-dev to run server development with typescript:

    yarn add -D ts-node-dev

### Add to package.json:

    "scrpit": {
        "dev": "ts-node-dev ./src/server.ts"
    },

## Run:

    yarn dev
