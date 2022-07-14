# mapframe
A set of helpful CSS components for creating web maps.

*MapFrame is under development, new changes may break previous versions*

## The Grid
The following code will create a CSS Grid layout which takes up the full extent of the viewport. Simply add the `mapframe-grid` class to the `body` element, and include the `header` and `main` semantic tags as children.

```html
<body class="mapframe-grid">
    <header>
        <! this is a header, put the title of the map here >
    </header>
    <main>
        <div class="--sidebar-l">
            <! this is a sidebar on the LEFT of the screen >
            <! it is OPTIONAL >
        </div>
        <div class="--main">
            <! this is the main content area >
            <! it is COMPULSORY >
        </div>
        <div class="--sidebar-l">
            <! this is a sidebar on the RIGHT of the screen >
            <! it is OPTIONAL >
        </div>
    </main>
</body>
```

By default, the grid is left visually unstyled. This is so you can use it to build your own styles on top.

Text styling is present for some semantic tags (`h1`, `h2`, `p`), no additional configuration is required. MapFrame uses Google Fonts to provide the Open Sans typeface.

## Pre-Built Components
If you're looking for more than just the grid itself, MapFrame also includes prebuilt elements of the UI, including a header and sidebar. This can be useful for quickly building a visual style which is easy to replace later.

MapFrame allows for both left and right sidebars, both of them can be visible at the same time if needed. Unfortunately, at this time, no accomodations are made for smaller screens.

### Header
Add the `mapframe-styled-header` class to the `header` element, for a quick visual header:

```html
<header class="mapframe-styled-header">
</header>
```

The header works great with a `<h1>` element, used for the map title.

### Sidebar
Add the `mapframe-styled-sidebar` class to a sidebar element (classed as either `--sidebar-l` or `--sidebar-r`).

```html
<div class="--sidebar-l mapframe-styled-sidebar">
</div>
```
The sidebar has a fixed width of 270px.