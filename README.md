# teardown-tstl-template

This template enables TypeScript support for mods in Teardown. The TypeScript isn't ran natively, it's compiled into Lua by [TSTL](https://typescripttolua.github.io).

## Files

- `src/` - TypeScript source files
- `dist/dist/mod` - Compiled Lua file and mod files.
- `assets/` - Generic assets such as vox files or sounds that are compiled into the mod.
- `info.txt` - The normal Teardown info.txt file, copied into the compiled mod.
- `teardown-ts-gen` - Submodule to the `decgen` branch of [teardown-ts-gen](https://github.com/yogwoggf/teardown-ts-gen). Adds the typed Teardown API to your TS environment.
- `tsconfig.json` - TypeScript configuration file, you shouldn't have to tinker with this much.

## How to compile

1. Go into `package.json` and customize the scripts to your liking (such as changing the folder name it copies to)
2. Run `npm run compile:windows` to build the mod, compile it all together, and then finally copy it to your Teardown `mods` directory (windows only)

You can delete all of the example files in `src/` and `assets/` if you want, they're just there to show you how it works.
