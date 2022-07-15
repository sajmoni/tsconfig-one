# tsconfig-one

## Highlights

- As strict as possible
- ESM output
- Only TypeScript allowed
- Forces usage of `import type`

## Usage

```sh
npm install --save-dev tsconfig-one
```

`tsconfig.json`

```json
{
  "extends": "tsconfig-one/tsconfig.json",
  "compilerOptions": {
    "outDir": "dist"
  },
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
