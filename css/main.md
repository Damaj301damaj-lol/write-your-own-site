# main.css

### CSS stands for Cascading Style Sheets, it is used to style the HTML elements, such as the color, the font, the size, and other stuff.

Here we are gonna define the properties of the text that is wrapped with the `<p>` tag.

```css
p {
    color: #000000;
    font-size: 10px;
}
```
All the text that is wrapped with the `<p>` tag will be black, and the font size will be 10px (10 pixels) and will use the system font.

Now let's define the properties of the text that is wrapped with the `<h1>` tag.

```css
h1 {
    color: #FFFFFF;
    font-size: 20px;
}
```
All the text that is wrapped with the `<h1>` tag will be white, and the font size will be 20px (20 pixels) and will use the system font.

### Tip: instead of repeating the same code for each tag, you can use a comma to separate the tags.

```css 
h1, h2, h3, h4, h5, h6 {
    color: #FFFFFF;
    font-size: 20px;
}
```
All the text that is wrapped with the `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>` tags will be white, and the font size will be 20px (20 pixels) and will use the system font.

### Tip: you can also use the `*` tag to apply the properties to all the tags.

```css 
* {
    color: #FFFFFF;
    font-size: 20px;
}
```
All the text that is wrapped with any tag will be white, and the font size will be 20px (20 pixels) and will use the system font.

You can also apply the propertices to classes, such as the `container` class.

```css
.container {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}
```
All the elements that have the `container` class will have a width of 100% of the screen, a height of 100% of the screen, will be displayed as a flexbox, will be centered horizontally, and will be centered vertically.

Rinse and repeat and you have a complete css file.