# Repolex Knowledge Graph of astropy/pytest-doctestplus

RDF knowledge graph data for [astropy/pytest-doctestplus](https://github.com/astropy/pytest-doctestplus), parsed by [repolex](https://repolex.ai).

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
rlex download astropy/pytest-doctestplus
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 019daf388a66ba5c672cb70dcdaa032181fe3749
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 019daf388a66ba5c672cb70dcdaa032181fe3749
│           └── chunk-001.nq.gz
├── blob
│   ├── 03ba7fd4682d52d9f3b0a07e931f633c3d40c66b.nq.gz
│   ├── 0454985815a23c4661583ff197cf666d9c646689.nq.gz
│   ├── 173059f9f457525760ad7c8dbc027bb40a469262.nq.gz
│   ├── 2119f51099bf37e4fdb6071dce9f451ea44c62dd.nq.gz
│   ├── 23393d6258c0d968db1c5c9e62a0a4b1c38c72be.nq.gz
│   ├── 2a7c0aa4122cadb7927e0f1b969fcf6dec784a09.nq.gz
│   ├── 2dd68fa1ae498d0eb869b9437b9ed7afd15a0cc7.nq.gz
│   ├── 2e7e58ff03b5d64e656245c9ef88987f1c10153a.nq.gz
│   ├── 53dd6f5b9156c294608c4ffabbc856ab4d3aa506.nq.gz
│   ├── 590e0b11e48c529682659b500d25455b75652009.nq.gz
│   ├── 5b8d50341a8676df84095c2e6f65b37ff4735d4c.nq.gz
│   ├── 5b9ea64334605a61052fe9636a915ccdb690d04c.nq.gz
│   ├── 6731cf1f4bd43875ad691725f37c484fc71502b9.nq.gz
│   ├── 7052c71e8b3b004ab8a5f52ad0a00a1ce1dfe4c7.nq.gz
│   ├── 72d48c047363401f6789bcbc13b7ac0d83400ef5.nq.gz
│   ├── 7fcc2f7462b9dc38beb562b75dd5c412558cb61a.nq.gz
│   ├── 878f0ec0d598aa219c97f7c2ade10f1f526c02c5.nq.gz
│   ├── 8b1e83363256c2def9bf969741280cc406dddaed.nq.gz
│   ├── 8cd32b82852b7beb7effe289c8a3cadf203cc0a3.nq.gz
│   ├── 8d2328010838497cccc32322f1fd9c8152bb312a.nq.gz
│   ├── 90fe83ee16a24749a0f3a619357c1289800ec7e4.nq.gz
│   ├── 91542cedbed2014233c4735037ba9f4acb832056.nq.gz
│   ├── 978f1d058551081305236c30dbd50f973e22c86f.nq.gz
│   ├── 9d871055853159a75a4360874c43700b0ec1da28.nq.gz
│   ├── a4b9b08b0283de1e1865999b0f53b357834ab582.nq.gz
│   ├── b507b35474ebf2eb9aeb41a0a0b918e0c6c1464b.nq.gz
│   ├── b743a72c590c75cca8e3ae12a565496820e13881.nq.gz
│   ├── b7c2aaabeda79aa977f6cfac4143b415123eddee.nq.gz
│   ├── c0c7064ec83ec8084c88d50651c8353acf0b0532.nq.gz
│   ├── c584119e61800e3c3182534aa4afcf5f82c4a4a7.nq.gz
│   ├── cba441a86700ea0e6d97c28b8834bdd9671a2354.nq.gz
│   ├── d4bb2cbb9eddb1bb1b4f366623044af8e4830919.nq.gz
│   ├── df79e8077de522311e73c6f9c939618a9c7abeef.nq.gz
│   ├── e311f7d73b4ab3f43c1f13edd89cebf327325a91.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e6d02b57a954219435707d83c5a13897881025c9.nq.gz
│   ├── e6dde014233f5cc81dc8d309b63541f4562834a4.nq.gz
│   ├── f30208948dfddca87e76ddda98a6ea415e3884aa.nq.gz
│   ├── f338b342b2cf02e9ef80b0834408444c5cfa7f9f.nq.gz
│   ├── f9df7c2e581842cbb306a017374bc70009fcf8f3.nq.gz
│   └── ff542b24aed83b47fc880410d8fd22841ff257cc.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 019daf388a66ba5c672cb70dcdaa032181fe3749.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 49 files
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

[astropy/pytest-doctestplus](https://github.com/astropy/pytest-doctestplus)

---
*Parsed on 2026-10-15 by [repolex](https://repolex.ai)*
