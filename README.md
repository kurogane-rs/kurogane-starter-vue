# Kurogane: Vue starter

A Vue 3 project scaffolded with Vite for Kurogane.

## Supported Languages

- `typescript`: Vue with TypeScript (`<script setup lang="ts">`), type checking via `vue-tsc`
- `javascript`: Vue with plain JavaScript (`<script setup>`), no type checking

## Usage with Kurogane CLI

```sh
kurogane new vue
```

Select a language when prompted.

## Non-interactive usage

```sh
cargo generate kurogane-rs/starter-vue --name my-app --define language=typescript
```

## What's included

- Vue 3 entry point with Composition API
- Vite with `@vitejs/plugin-vue`
- `vite.config.ts` configured to build into `content/`
- Rust binary using the Kurogane runtime
- `kurogane.toml` packaging configuration

## Development

```sh
npm install
npm run dev    # Start Vite dev server (port 5173)
kurogane dev   # Launch the Kurogane desktop app
```

## Building

```sh
npm run build     # Build frontend (includes vue-tsc for TypeScript)
kurogane build    # Build the Rust binary
```

## TypeScript vs JavaScript

The TypeScript variant includes `tsconfig.json` and uses `<script setup lang="ts">` in Vue components. The `build` script runs `vue-tsc -b` before Vite. The JavaScript variant uses `<script setup>` with no type checking.
