## (si no esta instalado el cli)

```
npm i -g @nestjs/cli
```

## iniciar un proyecto

```
nest new project-name
```

# Ó

## clonar repo

```
git clone https://github.com/sazukeR/graphql-nest-borrador.git
```

```
cd graphql-nest-borrador
```

```
yarn
```

```
yarn start:dev
```

## instalaciones realizadas en el proyecto

- graphql y apollo

```
yarn add @nestjs/graphql @nestjs/apollo @apollo/server graphql
```

- configurar apollo driver en el Module

```
GraphQLModule.forRoot<ApolloDriverConfig>({
 driver: ApolloDriver,
// debug: false,
 // playground: false
 autoSchemaFile: join( process.cwd(), 'src/schema.gql'),
 }),
```
