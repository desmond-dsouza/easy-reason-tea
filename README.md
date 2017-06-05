Quick Start to Create Reason TEA App
===

A way to start immediately with your Reason TEA app, with zero configuration.

1. `npm install -g bs-platform`
1. Clone this repo & `cd` into it
1. `npm link bs-platform` - symbolic links to global bs-platform
2. `npm install` - install all project & dev dependencies
3. `npm run dev` - build project & serve via local web server
4. Open browser and navigate to: http://localhost:8080/
5. Edit `src/app.re | index.re`, `public/index.html`
6. If auto-rebuild has no errors, browser will auto-reload


### Behind the scenes

`npm run dev` will:

1. ... run `bsb` in watch mode, which will compile your Reason code (and incrementally recompile it when needed), generating `.js` and other compiler-info files in the `lib/` directory.
2. ... in parallel, run webpack's dev server at http://localhost:8080/, bundling `bsb` and all other needed files in `public/` and serves them.




