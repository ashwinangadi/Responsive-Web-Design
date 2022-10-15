# Learn Basic CSS by Building a Cafe Menu
### Steps that are included to build a Cafe Menu, we learn all basics of CSS by completing this assignment.

## **Step 1**
As you learned in the last few steps of the Cat Photo App, there is a basic structure needed to start building your web page.

Add the `<!DOCTYPE html>` tag, and an `html` element with a `lang` attribute of `en`.

```html
<!DOCTYPE html>
<html lang="en">
  </html>
```

## **Step 2**
Add a `head` element within the `html` element, so you can add a `title` element. The `title` element's text should be `Cafe Menu`.

```html
<head>
  <title>Cafe Menu</title>
</head>
```

## **Step 3**
The `title` is one of several elements that provide extra information not visible on the web page, but it is useful for search engines or how the page gets displayed.

Inside the `head` element, nest a `meta` element with an attribute named `charset` set to the value `utf-8` to tell the browser how to encode characters for the page. Note that `meta` elements are self-closing.

```html
<head>
    <meta charset="utf-8">
    <title>Cafe Menu</title>
</head>
```

## **Step 4**
To prepare to create some actual content, add a `body` element below the `head` element.

```html
<head>
    <meta charset="utf-8" />
    <title>Cafe Menu</title>
</head>
<body>

</body>  
```

## **Step 5**
It's time to add some menu content. Add a `main` element within the existing `body` element. It will eventually contain pricing information about coffee and desserts offered by the cafe.

```html
<body>
    <main>

    </main>
</body>
```

## **Step 6**
The name of the cafe is `CAMPER CAFE`. Add an `h1` element within your `main` element. Give it the name of the cafe in capitalized letters to make it stand out.

```html
<main>
    <h1>CAMPER CAFE</h1>
</main>
```

## **Step 7**
To let visitors know the cafe was founded in 2020, add a `p` element below the `h1` element with the text `Est. 2020`.

```html
<h1>CAMPER CAFE</h1>
<p>Est. 2020</p>
```

