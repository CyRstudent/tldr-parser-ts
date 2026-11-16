---
title: ParseOptions
kind: interface
longname: ParseOptions
---

# ParseOptions

<Signature
  code="interface ParseOptions {
	allowedNAChars?: string[];
	binary?: string;
	client?: 'tlrc' | 'pythoncli';
	maxChar?: number;
	stripUsage?: boolean;
}"
/>

<SourceLink href="/source/src/types/clients-ts/#L54" label="clients.ts:54" />

---

## Properties

<MemberHeading id="allowednachars" depth="3" name="allowedNAChars" sig="allowedNAChars: string[]" />

<MemberMeta sourceHref="/source/src/types/clients-ts/#L79" sourceLabel="clients.ts:79" />

Array of allowed non-alphanumeric characters in a query

**Default:** `['+', '-']`

<MemberHeading id="binary" depth="3" name="binary" sig="binary: string" />

<MemberMeta sourceHref="/source/src/types/clients-ts/#L64" sourceLabel="clients.ts:64" />

Binary path to the executable if not available in PATH

**Default:** `'tldr'`

<MemberHeading id="client" depth="3" name="client" sig="client: 'tlrc' | 'pythoncli'" />

<MemberMeta sourceHref="/source/src/types/clients-ts/#L59" sourceLabel="clients.ts:59" />

The CLI tool to execute

**Default:** `'tlrc'`

<MemberHeading id="maxchar" depth="3" name="maxChar" sig="maxChar: number" />

<MemberMeta sourceHref="/source/src/types/clients-ts/#L74" sourceLabel="clients.ts:74" />

The max amount of characters allowed in a single query

**Default:** `50`

<MemberHeading id="stripusage" depth="3" name="stripUsage" sig="stripUsage: boolean" />

<MemberMeta sourceHref="/source/src/types/clients-ts/#L69" sourceLabel="clients.ts:69" />

Whether to remove the backticks from the examples

**Default:** `true`
