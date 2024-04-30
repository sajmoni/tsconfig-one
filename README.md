# tsconfig-one

## Highlights

- As strict as possible
- ESM output
- Forces usage of `import type`

_Requires TypeScript version >5.5_

## Usage

### Automatic (Recommended)

Use [setup-typescript](https://github.com/sajmoni/setup-typescript)

```console
npx setup-typescript@latest
```

### Manual

```console
npm install --save-dev tsconfig-one
```

`tsconfig.json`

```json
{
  "extends": "tsconfig-one/tsconfig.json",
  "include": ["src"]
}
```

### Application

Recommended additions if your project is an application:

```json
{
  "compilerOptions": {
    "incremental": true
  }
}
```
