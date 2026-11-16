[![CI](https://github.com/CyRstudent/tldr-parser-ts/actions/workflows/ci.yml/badge.svg)](https://github.com/CyRstudent/tldr-parser-ts/actions/workflows/ci.yml)
[![npm version](https://img.shields.io/npm/v/tldr-parser-ts)](https://www.npmjs.com/package/tldr-parser-ts)
[![npm downloads](https://img.shields.io/npm/dm/tldr-parser-ts)](https://www.npmjs.com/package/tldr-parser-ts)
[![License](https://img.shields.io/npm/l/tldr-parser-ts)](https://github.com/CyRstudent/tldr-parser-ts/blob/main/LICENSE)
[![Node.js](https://img.shields.io/node/v/tldr-parser-ts)](https://www.npmjs.com/package/tldr-parser-ts)
[![Documentation](https://img.shields.io/badge/docs-online-blue)](https://cyrstudent.github.io/tldr-parser-ts)

# tldr-parser-ts

A lightweight, TypeScript-based parser designed to convert [tldr](https://github.com/tldr-pages/tldr) markdown files into structured, type-defined data.
It extracts command name, description and examples, according to [their specification](https://github.com/tldr-pages/tldr?tab=contributing-ov-file#markdown-format)

---

## Features

- **Spec compliant**: Parses standard tldr pages according to their specification
- **Lightweight**: Only uses a single dependency, and the code has a minimal footprint!
- **Client support**: Support for multiple clients, and structural design so that adding more tldr clients is easy
- **Full customization for parsing**: Use the constraints you want for parsing queries!

---

## Prerequisites

This package relies on an installed `tldr` client to retrieve command pages. Ensure a supported CLI client (such as [`tlrc`](https://github.com/tldr-pages/tlrc)) is available in your machine:

```bash
# For OpenSUSE:
sudo zypper install tlrc
```

---

## Installation

Use whichever package manager suits you:
```bash
# npm
npm i tldr-parser-ts

# pnpm
pnpm add tldr-parser-ts
```

---

## Quick start

Import the parser, and pass a command name along with any configuration options:

```ts
import parse from 'tldr-parser-ts';

async function main() {
	const res = await parse('git merge', {
		stripUsage: false,
	});
	console.log(res);
}

void main();
```

---

## Development

First, set up the environment

```bash
git clone https://github.com/CyRstudent/tldr-parser-ts.git
cd tldr-parser-ts
pnpm install
```

When you're already set up:

```bash
# Run checks
pnpm check
pnpm typecheck
pnpm test:run

# Run Prettier & ESlint
pnpm run fix

# Build the package and its docs
pnpm build
pnpm docs:build # If you prefer, use pnpm docs:dev to set up a localhost with the page

```
