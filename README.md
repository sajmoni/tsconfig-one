# tsconfig-one

## :sparkles: Highlights

- As strict as possible
- ESM output
- Forces usage of `import type`

_Requires TypeScript version >5.5_

## :wrench: Usage

### Automatic (Recommended)

Use [setup-typescript](https://github.com/sajmoni/setup-typescript)

```console
npx setup-typescript@latest node|web|lib|base
```

### Manual

```console
npm install --save-dev tsconfig-one
```

`tsconfig.json`

```json
{
  "extends": "tsconfig-one/tsconfig.web.json",
  "include": ["src"]
}
```

### Configs

#### Lib

Use if your project is a library

```json
{
  "extends": "tsconfig-one/tsconfig.lib.json",
  "include": ["src"]
}
```

#### App - Node

Use if your project is a Nodejs application

```json
{
  "extends": "tsconfig-one/tsconfig.node.json",
  "include": ["src"]
}
```

#### App - Web

Use if your project is a Web application

```json
{
  "extends": "tsconfig-one/tsconfig.web.json",
  "include": ["src"]
}
```

#### Base

Only use this one if your for some reason cannot use any of the other ones

```json
{
  "extends": "tsconfig-one/tsconfig.base.json",
  "include": ["src"]
}
```
