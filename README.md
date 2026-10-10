# Repolex Knowledge Graph of pallets-eco/secure-cookie

RDF knowledge graph data for [pallets-eco/secure-cookie](https://github.com/pallets-eco/secure-cookie), parsed by [repolex](https://repolex.ai).

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
rlex download pallets-eco/secure-cookie
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── e06d58d068f2f6c4247886fca1a5afdfe140519e
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── e06d58d068f2f6c4247886fca1a5afdfe140519e
│           └── chunk-001.nq.gz
├── blob
│   ├── 00f3f64c07384272491cc08aa380259765f0aed7.nq.gz
│   ├── 0105a37c10bf947ad56fee55acd7a3066248db9c.nq.gz
│   ├── 017c5e372bdf0b9af5b3e80af63855d9d534bdcf.nq.gz
│   ├── 3bdc6911ac28e324b8ba3b8692bc2ea6ec78ec75.nq.gz
│   ├── 3cb7528e0ef51794fa1af709018a41ec5a20dc8c.nq.gz
│   ├── 49ec204104bfd3c894b37ab7e52b2ca079d25cb3.nq.gz
│   ├── 4a038904689b34669fa4a5a29819ac387d97fd84.nq.gz
│   ├── 4aae9f1b635ecb58bf0d9afc94ee5d008eb47ec5.nq.gz
│   ├── 51285967a7d9722c5bdee4f6a81c154a56aa0846.nq.gz
│   ├── 5b24333a378e4941e084f55feb67bf012d965600.nq.gz
│   ├── 5d9740b146f397879090635eba740cbb60e2a22e.nq.gz
│   ├── 673eb647389909e8774f3903e667a0e593ec8234.nq.gz
│   ├── 6cbb5cd5a80037e61f56fc6403ea11f7a9d5454b.nq.gz
│   ├── 7380b1b1fa65b7aeffeffe034829142d090ec9a0.nq.gz
│   ├── 760712c661b76df5e52813848f4cd91b8b64544a.nq.gz
│   ├── 7804b9029635072223535c718d77f7c42d505522.nq.gz
│   ├── 7893348a1b7dbb588983a48e6991282eae7e1b55.nq.gz
│   ├── 7a78554da62b8ec0d000cebf4b68ccd5d337162c.nq.gz
│   ├── 7be04e5548568a4c6d16cffa619fea51ec6ddcf0.nq.gz
│   ├── 955deaf27bc821a6367e818f36c016892fed3d33.nq.gz
│   ├── a53a98cf3d4b093c6696becd3df4e1c6c0660fc9.nq.gz
│   ├── b2d0bb480a2cb49b3220d1ce3cb4590301fd1e57.nq.gz
│   ├── b84b53d3aeb84a0cea17ea36ba235b1b9c2abd02.nq.gz
│   ├── b978f6645efb47c03e6e28ef7c4cbfa0c44f4597.nq.gz
│   ├── bc252819266b610f7c07a381cec512d50b2722c9.nq.gz
│   ├── c37cae49ec77ad6ebb25568c1605f1fee5313cfb.nq.gz
│   ├── d11881f41de23b808449e097d6ad8c134832f55c.nq.gz
│   ├── dec7c13c20b03c4d9f6f211f6a25ac70ae4ad518.nq.gz
│   ├── e079f8a6038dd2dc8512967540f96ee0de172067.nq.gz
│   ├── e32c8029d1860bf40125d8458db3bd1c4d3f4058.nq.gz
│   ├── e642e98a19694833255e4c640346b1d39c27a3c8.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ea0780999001240014b1801baf552b08787bd8aa.nq.gz
│   ├── f0bc28e10a45c5fba60aacbbf67363643d4f0fa7.nq.gz
│   ├── f1bd9903991ad93051b552094fa49b8cd9cb3fdb.nq.gz
│   ├── f3f1f01a6b12d7e8ff778745c0f6658b3845567b.nq.gz
│   ├── f4dd25bf6068bd6a6c3fcd0de159e4f9441c5d7f.nq.gz
│   └── f8aa3564dbe62412ae3e991e7122666d2dd79a60.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── e06d58d068f2f6c4247886fca1a5afdfe140519e.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 46 files
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

[pallets-eco/secure-cookie](https://github.com/pallets-eco/secure-cookie)

---
*Parsed on 2026-10-10 by [repolex](https://repolex.ai)*
