# Typescript Definitions For Electron

This is just what it says on the tin: the `electron.d.ts` from Electron's main distribution, minus the postinstall scripts.

(Why?  Because if you want to use Electron APIs when writing plugins for apps like [Obsidian](https://obsidian.md/), you don't need the Electron binaries, just the API definitions.)

Currently, the Electron version provided is 24.3.1, corresponding to the version used by the Obsidian 1.3.5 runtime, the previous major release of Obsidian.

Note: if you want VSCode to pick up these typings without an explicit `import "@ophidian/electron-types";`, install the package using alias under `@types` scope:

```
npm install @types/electron@npm:@ophidian/electron-types --save-dev
```

This should then be picked up by TypeScript without needing an explicit import.
