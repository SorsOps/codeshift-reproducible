```
npm init
npm i @backstage/codesmodes
```

`npm -v` - `9.5.0`
`node -v` - `v18.15.0`

`npm ls --depth 2`

```
└─┬ @backstage/codemods@0.1.44
  ├── @backstage/cli-common@0.1.12
  ├─┬ chalk@4.1.2
  │ ├── ansi-styles@4.3.0
  │ └── supports-color@7.2.0
  ├── commander@9.5.0
  ├─┬ jscodeshift-add-imports@1.0.10
  │ ├── @babel/traverse@7.21.4
  │ ├── jscodeshift-find-imports@2.0.4
  │ └── jscodeshift@0.11.0  <----
  └─┬ jscodeshift@0.14.0 <----
    ├── @babel/core@7.21.4
    ├── @babel/parser@7.21.4
    ├── @babel/plugin-proposal-class-properties@7.18.6
    ├── @babel/plugin-proposal-nullish-coalescing-operator@7.18.6
    ├── @babel/plugin-proposal-optional-chaining@7.21.0
    ├── @babel/plugin-transform-modules-commonjs@7.21.2
    ├── @babel/preset-env@7.21.4
    ├── @babel/preset-flow@7.21.4
    ├── @babel/preset-typescript@7.21.4
    ├── @babel/register@7.21.0
    ├── babel-core@7.0.0-bridge.0
    ├── chalk@4.1.2 deduped
    ├── flow-parser@0.203.1
    ├── graceful-fs@4.2.11
    ├── micromatch@4.0.5
    ├── neo-async@2.6.2
    ├── node-dir@0.1.17
    ├── recast@0.21.5
    ├── temp@0.8.4
    └── write-file-atomic@2.4.3
```

`./node_modules/jscodeshift` is @ 0.11.0 despite what the npm ls says despite what @backstage/codemodes specifies

```
//...
    "jscodeshift": "^0.14.0",
    "jscodeshift-add-imports": "^1.0.10"
//...
```