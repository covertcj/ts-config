# es-config

Simple, modern TypeScript tooling configuration common to many of my projects.

## Setup

Install `@covertcj/es-config` and it's peer dependencies:

```
npm i -D @covertcj/es-config @typescript-eslint/parser @typescript-eslint/eslint-plugin typescript eslint prettier eslint-config-prettier eslint-plugin-prettier
```

Then copy the config templates into your project:

```bash
cp "node_modules/@covertcj/es-config/templates/*" ./
```

And add an eslint runner to your `package.json`'s scripts:

```jsonc
{
  "scripts": {
    "lint": "tsc --noEmit && eslint --fix --ext .js,.ts src/"
  }
}
```
