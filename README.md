# Documentação do Projeto

## Instalações

### Instale o Typescript:

- Use o npm install typescript --save-dev ;


### Crie um arquivo tsconfig.json na raiz do seu projeto e configure as opções necessárias para o TypeScript (Não se esqueça de identa-lo):

{
  "compilerOptions": {
    "target": "es6",
    "module": "commonjs",
    "outDir": "./dist",
    "esModuleInterop": true,
    "sourceMap": true
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules", "**/*.spec.ts"]
}


## Alternativa:

- Caso você opitr por não instalar o ts-node globalmente, você pode instalá-lo localmente em seu projeto usando o comando npm install --save-dev ts-node.

- Em seguida, você precisará modificar o comando npm run dev em seu package.json usando:

"dev": "set NODE_ENV=dev&&nodemon ./src/server.ts",

## Transpilar o projeto:

- Para transpilar o projeto, rode o comando tsc ;

- Para rodar o projeto como TS, basta executar o comando: npm run dev
