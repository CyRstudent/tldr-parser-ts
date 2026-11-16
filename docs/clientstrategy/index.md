---
title: ClientStrategy
kind: interface
longname: ClientStrategy
description: The strategy to use depending on the client
---

# ClientStrategy

<Signature
  code="interface ClientStrategy {
	buildArgs: (queryArgs: string[]) => string[];
	isPageNotFound: (errmsg: string) => boolean;
}"
/>

<SourceLink href="/source/src/types/clients-ts/#L11" label="clients.ts:11" />

The strategy to use depending on the client

---

## Properties

<MemberHeading id="buildargs" depth="3" name="buildArgs" sig="buildArgs: (queryArgs: string[]) => string[]" />

<MemberMeta sourceHref="/source/src/types/clients-ts/#L17" sourceLabel="clients.ts:17" />

Function that generates the arguments passed onto execa

<MemberHeading id="ispagenotfound" depth="3" name="isPageNotFound" sig="isPageNotFound: (errmsg: string) => boolean" />

<MemberMeta sourceHref="/source/src/types/clients-ts/#L23" sourceLabel="clients.ts:23" />

Function to check, depending on the client and its output text, whether a page was not found
