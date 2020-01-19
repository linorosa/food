# Readme

Generates HTML with Pandoc.

Needs `jq`: https://stedolan.github.io/jq/

Hosting on the free Netlify plan automatically after a `git push`.

## Using

`./write Hello World` creates `recipes/hello-world.md`.
`./build` builds html from files under `recipes`.

## TODO

[ ] Take folder structure under /recipes into account while building index.html.
