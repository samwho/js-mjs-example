# js-mjs-example

This is a minimal JS project designed to showcase a problem.

Steps to reproduce:

```bash
# Install Bun (v1.0.7 at time of writing)
$ curl -fsSL https://bun.sh/install | bash

# Install dependencies
$ bun install

# Build out.js
$ bun run build
```

Now you'll have a file called `out.js` in the project root. If you open this
file and search for "DisplayObject.js" and "DisplayObject.mjs" you will find
that this class is included twice, once in a .js file and once in a .mjs file.
This isn't unique to this class, it seems there are lots of pixijs classes
included twice in this way.

Why? How do I prevent this?
