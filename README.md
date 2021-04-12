# Readme

Generates HTML with Pandoc.

Needs `jq`: https://stedolan.github.io/jq/

Hosting on the free Netlify plan automatically after a `git push`.
Hosting with Namecheap is a close second option. It's cheap, but not free.
Compress images with [Squoosh](https://squoosh.app/).

## Using

`./write Hello World` creates `recipes/hello-world.md`.
`./build` builds html from files under `recipes`.

## Template

```markdown
<!DOCTYPE html>
<html>
<head>
    <title>Granola Bars</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://unpkg.com/sakura.css/css/sakura.css" type="text/css">
    <link rel="stylesheet" href="../style7.css" />
<body>

<h1>Title</h1>
<hr/>

<h3>Ingredients:</h3>

<div>
    <span>1 cup <em>ingredient</em><div></div></span>
</div>

<h3>Instructions:</h3>

<ol>
    <li>
        A step with an inline ingredient of <span>1 cup <em>ingredient</em></span>.
    </li>
    <li>
        Another step with a list of ingredients:
        <div>
            <span>1 cup <em>ingredient</em><div></div></span>
        </div>
    </li>
</ol>

Originally seen at <a href="https://www.example.com">source</a>

</body>
</html>
```
