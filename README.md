## Start the project

    yarn init -y

## Create file .editorconfig with the content:

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

## Install typescript with dependency of development, run:

    yarn add -D typescript

## Configure typescript, run:

    yarn tsc --init

## Content for file tsconfig.json:

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

# Add Eslint, run:

    yarn add -D eslint
