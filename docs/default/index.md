---
title: default
kind: function
longname: default
description: The default function of the package, parsing the output of the tldr command
---

# default

<Signature code="default(query: string, options: ParseOptions): Promise<TLDRInfo>" />

<SourceLink href="/source/src/index-ts/#L23" label="index.ts:23" />

**Modifiers:** `async`

The default function of the package, parsing the output of the tldr command

**Parameters**

- `query` (string) — The command/subcommand to parse
- `options` ([ParseOptions](/parseoptions), default: `{}`) — Options to specify client used, binary path to the tool and whether stripped examples are wanted

**Returns**

- `Promise<`[`TLDRInfo`](/tldrinfo)`>` — A promise containing the parsed output as a TLDRInfo object.
