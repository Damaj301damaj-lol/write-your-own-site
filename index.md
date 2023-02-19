# index.php
This is the index file, it will be the first file to be loaded when someone visits the site.

First we start our file with the `<head>` tag, this is where we will put all the meta data for the site, such as the title, description, and other meta tags.

```html
<head>
    <title>My Site</title>
    <meta name="description" content="This is my site">
</head>
```

In the example above, we have added the title and description meta tags, you can add more meta tags if you want, such as keywords, author, and more.

However, you can also add other tags, such as `<link>` tags, which are used to link to external files, such as our css file and our favicon. Let's take our old example and add link tags to our files.

```html
<head>
    <title>My Site</title>
    <meta name="description" content="This is my site">
    <link rel="stylesheet" href="/css/main.css">
    <link rel="icon" href="/favicon.ico">
</head>
```
##### Note: these files will be created later, but for now, we will just add the tags.

##### Note: the `href` attribute is the path to the file, and the `rel` attribute is the relationship between the file and the site.

##### Note: While the `href` content doesn't neccecarily have to begin with a `/`, it is recommended to do so, this ensures that the file is loaded from the root of the site, and not from the current directory.

# Optional: do you want to have nice embeds when you share your site on social media? its easy!

Here is how to do it

```html
<head>
    <title>My Site</title>
    <meta name="description" content="This is my site">
    <link rel="stylesheet" href="/css/main.css">
    <link rel="icon" href="/favicon.ico">
    1. <meta content="#COLORS" data-react-helmet="true" name="theme-color" />
    2. <meta property="og:title" content="My Site">
    3. <meta property="og:description" content="This is my site">
    4. <meta property="og:image" content="/img/og-image.png">
    5. <meta property="og:url" content="https://example.com">
</head>
```
#### Note: those numbers are just to help you understand what each tag does, you shouldn't to add them in your final file.
Here is what each tag does:
1. This is the color of the bar at the top of the page on mobile devices, and is also the color of the link preview on social media. It accepts a hex color code, such as `#ff0000` or `#00ff00`.
2. This is the title of the site, it will be the title of the link preview on social media.
3. This is the description of the site, it will be the description of the link preview on social media.
4. This is the image of the site, it will be the image of the link preview on social media.
5. This is the url of the site, it will be the url of the link preview on social media.

## We finished writing the ``<head>`` part, we will now get onto the ``<body>`` part.

The ``<body>`` part is where we will put all the content of the site, such as the header, the main text, and the footer.

```html
</head>
<body>
    <h1>My Site</h1>
    <p>This is my site</p>
</body>
```
In this example, we have added a header (a title that has custom properties defined in our css file [will be created later]) and a paragraph, you can add more elements if you want

Now those will be shown on the top corner of our site, if we want this to be in the center, we can add a div with the class `container` and put all our content inside it.

```html
</head>
<body>
    <div class="container">
        <h1>My Site</h1>
        <p>This is my site</p>
    </div>
</body>
```

Same as example one, however its now in the middle of the page.

Let's do something more advanced, let's add a header and a footer to our site.

Header: the content on the top of your site, usually contains the logo, the navigation bar, and other stuff, is persistent across all pages.

Footer: the content on the bottom of your site, usually contains the copyright, the social media links, and other stuff, is persistent across all pages.

We will use the <?php include> command to include the header and footer files, which will be created later.

```html
</head>
<body>
    <div class="container">
        <?php include "/templates/header.php"; ?>
        <h1>My Site</h1>
        <p>This is my site</p>
        <?php include "/templates/footer.php"; ?>
    </div>
</body>
```
You can add more content, such as images, let's add one!
    
```html
</head>
<body>
    <div class="container">
        <?php include "/templates/header.php"; ?>
        <h1>My Site</h1>
        <p>This is my site</p>
        <img src="/img/image.png" alt="My Site">
        <?php include "/templates/footer.php"; ?>
    </div>
```

`<img>` is used to add an image to the site, the `src` attribute is the path to the image, and the `alt` attribute is the alternative text, which is shown if the image fails to load.

Let's add a hyperlink to our site, so that when someone clicks on it, they will be redirected to another page.

```html
</head>
<body>
    <div class="container">
        <?php include "header.php"; ?>
        <h1>My Site</h1>
        <p>This is my site</p>
        <img src="/img/image.png" alt="My Site">
        <a href="/about">About</a>
        <?php include "footer.php"; ?>
    </div>
```

`<a>` is used to add a hyperlink to the site, the `href` attribute is the path to the page, and the content of the tag is the text that will be shown.

In the example above, we have added a link to the about thing, it can be a file or a folder, if a folder is specified, the index file will be loaded.

We have finished writing our index file.

Move to an other file, i recommend you start with the css file.
