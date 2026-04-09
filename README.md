# Repolex Knowledge Graph of sweepline/eslint-plugin-unused-imports

RDF knowledge graph data for [sweepline/eslint-plugin-unused-imports](https://github.com/sweepline/eslint-plugin-unused-imports), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download sweepline/eslint-plugin-unused-imports
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 8b3486a2a38071573a607f6f6b92c3f0e56887f1
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 8b3486a2a38071573a607f6f6b92c3f0e56887f1.nq.gz
│   └── repolex
│       └── 8b3486a2a38071573a607f6f6b92c3f0e56887f1
│           └── chunk-001.nq.gz
├── blob
│   ├── 1b0a5742973115d63245be72edcd3716c3dd3512.nq.gz
│   ├── 2abf2b7234a7b855d451c7ea37a3f13b45176bba.nq.gz
│   ├── 4f772037cd3bf2eb06dc74d2a4b06c35ea1e38fb.nq.gz
│   ├── 635566f805447d15a704f795e8327b03a3fe54fb.nq.gz
│   ├── 64fbe6ac017d5cc423e3377c26b3b37dcc8c45e9.nq.gz
│   ├── 7527018372692a1888726a60291087af68bf36dd.nq.gz
│   ├── 82afa9936113a119383f21537d53592952ac5a20.nq.gz
│   ├── 854dd973134f38bf2e035494401fb0a14680c4f1.nq.gz
│   ├── 8b1c61f31952ba990f595e6b9c2f5e8d9f543695.nq.gz
│   ├── 8bea256a63f9c2578fdedc636828cc5b148289cf.nq.gz
│   ├── 9c1fc43cc7d1020c0fe3500ed5684c1a383a8599.nq.gz
│   ├── 9e01a3690ba186313fc94fd2de1f80bbb0a0cf19.nq.gz
│   ├── a128733be256fe6e5e634bcb3e9ec773dc4df173.nq.gz
│   ├── af899580c666d1cc0bd654c8e5e4b65e20506fe8.nq.gz
│   ├── b15238fc59e03b1ccc0d9ef6fd3fc7bfe92d8c7b.nq.gz
│   ├── b5e61eb7615422feab5421f554f098ef6a2df568.nq.gz
│   ├── b8ed38ce1be2dc1226189091ebc34ab008c433d2.nq.gz
│   ├── b975ef2b7ae7b00e12a579caf67a7c5146829c11.nq.gz
│   ├── cf05326b9404dee2db31de9b0b984e3215b753e1.nq.gz
│   ├── cf69529a5314ca3d5660864cb34a360d8660b269.nq.gz
│   ├── efc037aa8467135a1f3578711c4bf2240aff1cb3.nq.gz
│   ├── f9156abdfad32f8290349f512f46ee5ebcf6eaef.nq.gz
│   └── fc2a9d3fc4ce6094434b31ff0005fe78ff3d9047.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 8b3486a2a38071573a607f6f6b92c3f0e56887f1.nq.gz
├── filetree
│   └── 8b3486a2a38071573a607f6f6b92c3f0e56887f1.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 33 files
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

## Source repository

[sweepline/eslint-plugin-unused-imports](https://github.com/sweepline/eslint-plugin-unused-imports)

---
*Parsed on 2026-04-09 by [repolex](https://repolex.ai)*
