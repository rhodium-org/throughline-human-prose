# Human prose — avoid AI-writing tells — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates
it in CI. The prose headings are hand-owned — everything between `tl:*` markers is
injected from the YAML items, so the published spec can never drift from the graph.

This source is the **human prose axis**: write so the text does not read as machine
generated. It is the neutral or opposite form of the tells catalogued in Wikipedia's
"Signs of AI writing" advice page. It deliberately reinforces neighbouring axes
(readability, register, spelling conventions) but from a distinct intent — removing the
statistical fingerprint of generated text — and governs nothing about readability
targets, register, spelling, genre, medium or brand voice, each of which is its own
throughline source. Every principle is a `user_requirement`; every rule is a
`system_requirement` that `implements` its principle. The throughline UIDs are this
source's own and immutable — a consumer cites a rule as `human:SR-0001`.

It carries
<!-- tl:count type == 'user_requirement' -->
8
<!-- tl:end --> principles and
<!-- tl:count type == 'system_requirement' -->
30
<!-- tl:end --> rules.

## Purpose

<!-- tl:item INT-0001 -->
**INT-0001 — Prose reads as human-written, not machine-generated** — `intent`, status `approved`

> Large language models regress to the mean; their output carries a recognisable statistical fingerprint — inflated significance, vague authority, formulaic parallelisms, a narrow flagged vocabulary, mechanical emphasis, leftover assistant framing and unverifiable citations. This axis governs the removal of that fingerprint: it names each observed tell and states the plain human alternative. It is the neutral or opposite form of the patterns catalogued in Wikipedia's "Signs of AI writing" advice page. It deliberately reinforces neighbouring axes (readability, register, spelling conventions) but from a distinct intent — two texts equally clear, neutral and correctly spelled can still differ in whether they read as generated, and that difference is what this axis owns.

**source_ref**: TBS Human prose
<!-- tl:end -->

## 1. Keep specific facts specific; do not inflate significance

<!-- tl:item UR-0001 -->
**UR-0001 — Keep specific facts specific; do not inflate significance** — `user_requirement`, status `approved`

> State the concrete, particular fact rather than a generic, important-sounding summary; do not add claims about the subject's significance, legacy or place in a broader trend that the sources do not make.

*Derives from:* INT-0001

**source_ref**: TBS Human prose — Significance and puffery
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0001' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | approved | Give the specific fact, not a generic important-sounding summary |
| SR-0002 | system_requirement | approved | Do not assert broader significance the sources do not claim |
| SR-0003 | system_requirement | approved | Describe plainly; avoid promotional and travel-guide language |
| SR-0004 | system_requirement | approved | Do not end with a formulaic challenges-and-future-prospects passage |
<!-- tl:end -->

## 2. Attribute claims to named sources, not vague authorities

<!-- tl:item UR-0002 -->
**UR-0002 — Attribute claims to named sources, not vague authorities** — `user_requirement`, status `approved`

> Attribute every opinion or contested claim to a specific, named source, and do not overstate how many sources hold a view or editorialise about a subject's notability or coverage.

*Derives from:* INT-0001

**source_ref**: TBS Human prose — Attribution
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0002' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0005 | system_requirement | approved | Name the source of an opinion; avoid vague authorities |
| SR-0006 | system_requirement | approved | Do not overstate how widely a view is held |
| SR-0007 | system_requirement | approved | State facts, not the case for the subject's notability |
<!-- tl:end -->

## 3. Let analysis come from substance, not tacked-on filler

<!-- tl:item UR-0003 -->
**UR-0003 — Let analysis come from substance, not tacked-on filler** — `user_requirement`, status `approved`

> Do not append hollow analytical flourishes that assert importance, impact or connection without saying, concretely and from a source, what they are.

*Derives from:* INT-0001

**source_ref**: TBS Human prose — Analytical filler
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0003' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0008 | system_requirement | approved | Do not tack a significance clause onto the end of a sentence |
| SR-0009 | system_requirement | approved | Do not claim significance without saying what it is |
<!-- tl:end -->

## 4. Vary sentence structure; avoid formulaic patterns

<!-- tl:item UR-0004 -->
**UR-0004 — Vary sentence structure; avoid formulaic patterns** — `user_requirement`, status `approved`

> Avoid the repeated structural mannerisms of generated text — corrective negative parallelisms, the rule of three, and needless synonym variation — and let the number and shape of clauses follow the content.

*Derives from:* INT-0001

**source_ref**: TBS Human prose — Sentence patterns
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0004' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0010 | system_requirement | approved | Avoid corrective negative parallelisms |
| SR-0011 | system_requirement | approved | Do not force ideas into threes |
| SR-0012 | system_requirement | approved | Repeat the right word rather than varying it for its own sake |
<!-- tl:end -->

## 5. Use plain, direct verbs and ordinary vocabulary

<!-- tl:item UR-0005 -->
**UR-0005 — Use plain, direct verbs and ordinary vocabulary** — `user_requirement`, status `approved`

> Prefer the simple copula and the ordinary word to the flagged register of generated prose — its avoidance of "is" and "has", and its recurring vocabulary of delve, tapestry, testament, underscore, pivotal, robust and the like.

*Derives from:* INT-0001

**source_ref**: TBS Human prose — Vocabulary and verbs
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0005' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0013 | system_requirement | approved | Use the plain copula; do not avoid "is", "are" and "has" |
| SR-0014 | system_requirement | approved | Avoid the flagged AI-vocabulary register |
| SR-0015 | system_requirement | approved | Prefer the plain verb to its stiff synonym |
<!-- tl:end -->

## 6. Emphasise and format with restraint

<!-- tl:item UR-0006 -->
**UR-0006 — Emphasise and format with restraint** — `user_requirement`, status `approved`

> Avoid the mechanical formatting habits of chatbot output — Title Case headings, pervasive boldface, everything-as-a-bullet-list, dense em dashes and decorative emoji — and reserve emphasis and structure for where the content genuinely needs it.

*Derives from:* INT-0001

**source_ref**: TBS Human prose — Emphasis and formatting
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0006' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0016 | system_requirement | approved | Write headings in sentence case |
| SR-0017 | system_requirement | approved | Use boldface sparingly, for genuine emphasis only |
| SR-0018 | system_requirement | approved | Do not turn prose into bold-header bullet lists |
| SR-0019 | system_requirement | approved | Use dashes at ordinary density |
| SR-0020 | system_requirement | approved | Do not use emoji as bullets or heading decoration |
| SR-0021 | system_requirement | approved | Do not build a table where prose would do |
<!-- tl:end -->

## 7. Leave no machine, draft or conversational artifacts in the text

<!-- tl:item UR-0007 -->
**UR-0007 — Leave no machine, draft or conversational artifacts in the text** — `user_requirement`, status `approved`

> The finished piece addresses its reader, not a chatbot's operator: strip assistant-to-user framing, knowledge-cutoff and availability disclaimers, tool and citation markup, unfilled placeholders and restated summaries.

*Derives from:* INT-0001

**source_ref**: TBS Human prose — Artifacts and framing
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0007' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0022 | system_requirement | approved | Remove assistant-to-user framing |
| SR-0023 | system_requirement | approved | Include no knowledge-cutoff or availability disclaimers, and do not speculate to fill gaps |
| SR-0024 | system_requirement | approved | Leave no tool or citation markup artifacts in the text |
| SR-0025 | system_requirement | approved | Fill in or delete every placeholder |
| SR-0026 | system_requirement | approved | Do not add a restating summary paragraph |
| SR-0027 | system_requirement | approved | Drop didactic "it is important to note" disclaimers |
<!-- tl:end -->

## 8. Cite only real, verifiable, specific sources

<!-- tl:item UR-0008 -->
**UR-0008 — Cite only real, verifiable, specific sources** — `user_requirement`, status `approved`

> Every reference must point to a source that exists, that you have checked, and that supports the claim; give enough locating detail to verify it, and cite nothing you cannot.

*Derives from:* INT-0001

**source_ref**: TBS Human prose — Citations
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0008' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0028 | system_requirement | approved | Cite only sources you have verified exist and support the claim |
| SR-0029 | system_requirement | approved | Give enough locating detail to verify each citation |
| SR-0030 | system_requirement | approved | Ensure every reference is cited and every citation resolves |
<!-- tl:end -->
