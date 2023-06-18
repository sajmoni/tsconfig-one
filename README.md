# tsconfig-one

## Highlights

- As strict as possible
- ESM output
- Only TypeScript allowed
- Forces usage of `import type`
- Enables absolute imports

## Usage

```console
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

### Absolute imports

Import files with `~/`

**Example**

`src/example.ts` -> `~/example`

**vite**

If using `vite`, add this to your `vite.config.ts`

```ts
resolve: {
    alias: {
      '~': resolve(__dirname, 'src'),
    },
  },
```
