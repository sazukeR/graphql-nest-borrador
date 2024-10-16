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

```
http://localhost:3000/graphql
```

## instalaciones realizadas en el proyecto

- graphql y apollo

```
yarn add @nestjs/graphql @nestjs/apollo @apollo/server graphql
```

- instalar apollo server core

```
yarn add apollo-server-core
```

- configurar apollo driver en el Module

```
GraphQLModule.forRoot<ApolloDriverConfig>({
 driver: ApolloDriver,
// debug: false,
  playground: false,
 autoSchemaFile: join( process.cwd(), 'src/schema.gql'),
  plugins: [ApolloServerPluginLandingPageLocalDefault()],
 }),
```

## para generar un recurso ej:

```
nest g res todos --no-spec
```
