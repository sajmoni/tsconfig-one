# tsconfig-one

## Highlights

- As strict as possible
- ESM output
- Only TypeScript allowed
- Fast (incremental)

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
