Quick Start to Create Reason TEA App
===

A way to start immediately with your Reason TEA app, with zero configuration.

1. Clone this repo
2. `npm install`
3. `npm run dev`
4. Open browser and navigate to: http://localhost:8080/
5. Edit `src/app.re` and/or `src/index.re` and save.
6. If auto-rebuild has no errors, browser will auto-reload


### Behind the scenes

`npm run dev` will:

1. ... run `bsb` in watch mode, which will compile your Reason code (and incrementally recompile it when needed), generating `.js` and other compiler-info files in the `lib/` directory.
2. ... in parallel, run webpack's dev server at http://localhost:8080/, bundling `bsb` and all other needed files in `public/` and serves them.




