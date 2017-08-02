This repo contains several packages to demonstrate apmjs usage.

## Source Tree

This repo contains 3 different packages: `demo-hello`, `demo-world`, and `demo-workspace`:

```
.
├── README.md
├── demo-hello
│   ├── index.js
│   └── package.json
├── demo-workspace
│   └── package.json
└── demo-world
    ├── index.js
    └── package.json
```

## Dependency Tree

The dependency tree is as follows:

```
demo-workspace
├── foo
└── @jetwg/demo-world
    └── @jetwg/demo-hello
```

## Installation

Install `apm` first:

```bash
npm install -g apmjs
```

Install dependencies for `demo-workspace`:

```bash
cd demo-workspace
apm install
```

All dependencies will be installed in `amd_modules`, and `amd_modules/index.json` contains a mapping for all modules.
