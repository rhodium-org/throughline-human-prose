# throughline-human-prose

The **human prose** content axis — write so the text does **not** read as machine
generated — expressed as a [throughline](https://pypi.org/project/throughline/)
**source**: a standalone, grounded requirements graph that a consuming project composes with
`tl` from [throughline](https://pypi.org/project/throughline/) 3.11.0 or later.

This repository holds no application code. It is a directory of small YAML items with
permanent UIDs, validated by `tl check`. Consumers import it under a namespace and
reference its rules as `human:SR-0001` or its principles as `human:UR-0001`.

## What this axis is

Large language models regress to the mean, and their output carries a recognisable
statistical fingerprint. This source is a field guide of that fingerprint's tells,
each rewritten as the plain human alternative. The tells are drawn from Wikipedia's
[*Signs of AI writing*](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
advice page (WikiProject AI Cleanup); every rule here states the neutral or opposite
form of a pattern catalogued there.

## One orthogonal axis

This axis owns one thing: **removing the fingerprint of generated text**. It
deliberately *reinforces* its neighbours but is not any of them, because two pieces of
writing can be equally clear, neutral and correctly spelled and still differ in whether
they read as generated. It says nothing about:

- **readability** (word choice, sentence length, active voice) — `throughline-plain-language`
- **register** (formal / neutral / informal) — `throughline-tone-*`
- **conventions** (spelling, punctuation, capitalisation, numbers) — `throughline-conventions-uk`
- **genre / purpose** (inform, instruct, persuade) — `throughline-purpose-*`
- **medium / channel** (web page, letter, email) — `throughline-medium-*`
- **audience** (general, practitioner, expert) — `throughline-audience-*`

A task like *"a plain, formal, UK-English web page that does not read as AI-written"*
becomes a **compose** of `plain` + `tone-formal` + `conventions-uk` + `medium-web` +
`human`.

## What's in the graph

<!-- tl:count type == 'user_requirement' -->
8
<!-- tl:end --> principles as `user_requirement`s, each `derives_from` the root
intent, and
<!-- tl:count type == 'system_requirement' -->
30
<!-- tl:end --> rules as `system_requirement`s, each `implements` its principle. The
published spec is generated from the graph at [`docs/spec.md`](docs/spec.md).

## Source & licensing

The rules are original house guidance, licensed under Apache-2.0. They reproduce no
third-party standard: the Wikipedia page is cited as the source of the *observations*
only, under CC BY-SA, and none of its text is copied here. Each rule records its
dimension in `attrs.source_ref` and its owning principle in `attrs.principle`. See
[`NOTICE`](NOTICE).

## Extending the source

Items are hand-authored static YAML — one file per item, one permanent UID per file.
To add a rule, create the next `SR-00NN.yml` by hand (never renumber an existing one)
and link it with `implements` to its principle. Then:

```sh
tl check --strict      # the graph must stay sound
tl docs                # regenerate docs/spec.md + README.md
tl docs --check        # CI gate: docs must match the graph
```
