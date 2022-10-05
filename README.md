# <center> 🧑‍💻 HTML-CHEATSHEET 🌐 </center>

## Base elements -

The HTML elements that allow you to build the most basic web page

<br>

## html

Defines the root element of an HTML document. All other elements must be contained within this root element.

<br>

## head

Defines a container for a web page's metadata.

<br>

## body

The container for a web page's content. Must be a direct child of `<html>`, and must be an ancestor of all HTML elements (except where noted).

<br>

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Document metadata -->
  </head>
  <body>
    <!-- Document content -->
  </body>
</html>
```

<hr>
<br>

## link

Defines a link between the current web page and an external link or resource.

```html
<link
  rel="stylesheet"
  type="text/css"
  href="https://htmlreference.io/css/website.css"
/>
```

Description :

### `href`

Defines the URL of the link.

- = `"https://htmlreference.io/css/website.css"`
  - You can pass an absolute URL like above.
- = `href="/css/website.css"`
  - You can pass a URL relative to the root

<br>

### `rel`

Defines a link type, explaining how the link relates to the current web page.

- = `"stylesheet"`
  - The link is a stylesheet.
- = `"icon"`
  - The link is a favicon.
- = `"author"`
  - The link is the web page's author website.
- = `"next"`
  - The link is the next page.

<br>

### `type`

Defines the type of the linked resource.

- = `"text/css"`
  - The link is a CSS file.
- = `"text/html"`
  - The link is an HTML document.

<hr>
<br>

## meta

Defines metadata attached to a web page.

```html
<meta charset="UTF-8" />
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<meta name="theme-color" content="#ffffff" />
```

```html
<!-- Refresh the page every 5 seconds -->
<meta http-equiv="refresh" content="5" />
```

```html
<!-- Redirect instantly to https://saawn.dev -->
<meta http-equiv="refresh" content="0; url=https://saawn.dev" />
```

### `charset`

Defines the character encoding for the whole web page.

- = `"UTF-8"`
  - The value must be a valid [character set.](https://www.iana.org/assignments/character-sets/character-sets.xhtml)

### `http-equiv`

Defines meta rules for the web page.

- = `"Content-Security-Policy"`
  - Defines a link to a web page's content policies.
- = `"refresh"`
  - Allows to refresh the web page every N seconds, or even redirect to another URL.
- = `"X-UA-Compatible"`
  - Defines which Internet Explorer verison the web page should be rendered as.

### `name`

Defines additional information attached to the web page.

- = `"viewport"`
  - Defines dimension and scaling rules for the viewport.
- = `"theme-color"`
  - Defines a theme color which can be used by the browser or the operating system.

### `content`

Defines the content of the metadata. This varies according to the name or http-equiv value.

- = `"width=device-width, initial-scale=1"`
  - For the viewport metadata, you can specify the width and initial scale of the web page.
- = `"2; url=https://saawn.dev"`
  - For the refresh metadata, you can specify how many seconds to wait before redirecting to another URL.

<hr>
<br>

## script

Defines a container for an external script.

```html
<script src="https://htmlreference.io/javascript/my-scripts.js"></script>
```

```html
<script type="text/javascript">
  console.log("Hello World");
</script>
```

### `src`

Defines the source of the external script.

- = `src="/javascript/my-scripts.js"`
  - The URL can be relative or absolute

### `type`

Defines the [MIME](https://www.iana.org/assignments/media-types/media-types.xhtml) type of the external script.

- = `type="text/javascript"`
  - This is for `.js` files.

### `async`

Allows the external script to be loaded asynchronously.
No value required.

<hr>
<br>
