# 📔 [Localize]

This **[Astro integration][astro-integration]** allows you to translate your
components using InLang.

## Installation

There are two ways to add integrations to your project. Let's try the most
convenient option first!

### `astro add` command

Astro includes a CLI tool for adding first party integrations: `astro add`. This
command will:

1. (Optionally) Install all necessary dependencies and peer dependencies
2. (Also optionally) Update your `astro.config.*` file to apply this integration

To install `Localize`, run the following from your project directory and
follow the prompts:

Using NPM:

```sh
npx astro add inlang-astro
```

Using Yarn:

```sh
yarn astro add inlang-astro
```

Using PNPM:

```sh
pnpx astro add inlang-astro
```

### Install dependencies manually

First, install the `Localize` integration like so:

```sh
npm install -D -E inlang-astro
```

Then, apply this integration to your `astro.config.*` file using the
`integrations` property:

**`astro.config.ts`**

```ts
import inlang from "inlang-astro";

export default { integrations: [inlang()] };
```

## Getting started

#### Set `Logger` to `0` if you do not want to see debug messages. Default is `2`.

**`astro.config.ts`**

```ts
import inlang from "inlang-astro";

export default {
	integrations: [
		inlang({
			Logger: 0,
		}),
	],
};
```

[Localize]: https://npmjs.org/inlang-astro
[astro-integration]: https://docs.astro.build/en/guides/integrations-guide/

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for a history of changes to this integration.
