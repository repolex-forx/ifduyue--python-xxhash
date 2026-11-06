# Repolex Knowledge Graph of ifduyue/python-xxhash

RDF knowledge graph data for [ifduyue/python-xxhash](https://github.com/ifduyue/python-xxhash), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download ifduyue/python-xxhash
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 54c863576b0ee517cfa3a276e0f6c15ea016bc27
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 54c863576b0ee517cfa3a276e0f6c15ea016bc27
│           └── chunk-001.nq.gz
├── blob
│   ├── 0030f445f0ef1595e7ea9e329114230492836960.nq.gz
│   ├── 0b5d5e4b6abd63495656e2f664a95eb2ded4ea03.nq.gz
│   ├── 0d08e261a2ae9d87844cc5092013cf01f98b301d.nq.gz
│   ├── 1bb12ac43f4c970b78e6d4894cf694ba7c794101.nq.gz
│   ├── 24584a338e4b598f5fd0a455ba40e84670d68925.nq.gz
│   ├── 24852ba4da4986eaa2a3a3e0d9fc2fc14f3004af.nq.gz
│   ├── 2cc6eafecaccf77f72343475a311ff3bb821a5de.nq.gz
│   ├── 351d9a7db537b56896cec1764086c7486ed397cb.nq.gz
│   ├── 37d5bf60f6405c4e55afe2e55f3462f2bc4ff0f6.nq.gz
│   ├── 3a66f7115e6957f95b3a0bd18edb8988663c7234.nq.gz
│   ├── 3c3f1fd6fb530a0e8c94b6b69b13197b0b3cb9e8.nq.gz
│   ├── 435152ca9f348759f7d399b1345f5884f59b2612.nq.gz
│   ├── 4825901ec5540cecb8e20a1fadda73f1b69a19b3.nq.gz
│   ├── 49732953ce9beae18f940160daecd55035f5c2ce.nq.gz
│   ├── 64e376e034f4325385551043004925ed2189ab9e.nq.gz
│   ├── 6f4da738cd40740259d8ea7367ae0c321bd49d74.nq.gz
│   ├── 70b7d276937175fdc9ead587b95f3f964ec73942.nq.gz
│   ├── 7eee9065e1ef1459c88861646e6558a9a1c2288a.nq.gz
│   ├── 8256db647dd5a41d023d6ce0b2513f0627754ad0.nq.gz
│   ├── 963b1182eea4863d861c40a43099031a7e0e8fc9.nq.gz
│   ├── 9a18251d4cb4563e5c133eb10749154bb3bf8f10.nq.gz
│   ├── a2254e11f3012e1996e24883a80e126e7adb45e7.nq.gz
│   ├── a6df97794168c7e260802ca99a4b8b7baa9f729b.nq.gz
│   ├── ab6cd8fb165480686771a70b5b45c334bfd8388b.nq.gz
│   ├── b8e20f0298819ac55d76401b77d772aaf018a713.nq.gz
│   ├── c643b95c3c8fa92eb80f95188981c37165ad7e27.nq.gz
│   ├── d2acc5594e2ea72fcf77369e7c4119f5212b97cf.nq.gz
│   ├── d515798c1663f061280ffdc7cfa2ca56fad4d169.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── f8fd479ccbfdf08e1c1e2f1e3837bae9633cf39d.nq.gz
│   ├── f919d2acc000ab5ac18cdc6dfc40800cbc83bebd.nq.gz
│   └── fa21b90cca47d1acd1176bdaa7b6272b22954778.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 54c863576b0ee517cfa3a276e0f6c15ea016bc27.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 40 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[ifduyue/python-xxhash](https://github.com/ifduyue/python-xxhash)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
