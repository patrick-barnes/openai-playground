# OpenAI Playground

Just a POC to become familiar with OpenAI libraries.

Asks ChatGPT to write a haiku, such as:

```
Function calls again,
Layers deep, a loop unfolds,
Self calls to the end.
```

## Usage

1. Set `OPENAI_API_KEY` environment variable.
2. `node app`

## How it works

- Configures ChatGPT: "You are a helpful assistant."
- Asks ChatGPT: "Write a haiku about recursion in programming."

Example output:

```json
{
  role: 'assistant',
  content: 'Function calls again,  \n' +
    'Layers deep, a loop unfolds,  \n' +
    'Self calls to the end.',
  refusal: null
}
```

## Appendix

### `*.mjs` vs `*.js`

- `.mjs` = always ES Module format
- `.js` = ES Module or CommonJS, depending on the type in `package.json`

### ES Module vs CommonJS

- ES Module = modern, uses `import`
- CommonJS = older, uses `require`
