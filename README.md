A LESS port of Bootstrap 4.3.1 grid system. No Javascript.

# Usage

Compile the grid yourself with

```
npm i
npm run dist
```

It generates two files: `grid.css` and `dist/grid.css`.
The second one should be used for production.

Import the file `dist/grid.css` to your HTML5 page as a simple stylesheet

```
<link rel="stylesheet" type="text/css" href="dist/grid.css">
```

use it with the same syntax as bootstrap grid.

# Demo

Here is the content of `demo.html` file:

```
<!DOCTYPE html>
<html>
    <head>
        <title>demo</title>
        <link rel="stylesheet" type="text/css" href="grid.css">
    </head>
    <body>
        <div class="container">
            <div class="row">
                <div class="col" style="background: aqua;">1</div>
                <div class="col" style="background: coral;">2</div>
                <div class="col" style="background: aqua;">3</div>
            </div>
            <div class="row">
                <div class="col" style="background: coral;">1</div>
                <div class="col-6" style="background: aqua;">2</div>
                <div class="col" style="background: coral;">3</div>
            </div>
        </div>
        <div class="container">
            <div class="row">
                <div class="col-sm-8">col-sm-8</div>
                <div class="col-sm-4">col-sm-4</div>
            </div>
            <div class="row">
                <div class="col-sm">col-sm</div>
                <div class="col-sm">col-sm</div>
                <div class="col-sm">col-sm</div>
            </div>
        </div>
    </body>
</html>
```

# You should know

In `grid.less` I changed the values of the grid to match SAP Fiori 3 grid specifications.
This is a 16 columns grid and its breakpoints are different than bootstrap.

- <https://getbootstrap.com/docs/4.1/layout/grid/#customizing-the-grid>

⚠️ I did port only the essential stuff. There might be some features you might want to implement yourself

# Final thought

This was a challenge I gave to myself, I did this over a weekend and for external reasons never merged it on the project I work on. This was fun to implement though.

This might be of use for people who have a large less legacy and won't switch to sass.

Finally, if you have the choice to use sass on your project, you can extend the grid easily, have a look at <https://getbootstrap.com/docs/4.1/getting-started/theming/>
