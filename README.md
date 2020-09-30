# Brand Style Guide.

Welcome to the Brand Style Guide! A tool for creating and maintaining style guides easily.


## Introduction.

This guide consists of an HTML-document with a linked CSS style sheet. The brand style guide can be used as is to visually show clients their style brand and, for example, making a simple one-page website they can use to refer back to their brand design, for instance, with the help of GitHub pages.


## How to use.

### 1. Change company identity

- In the `<script>` tag in `index.html`, change the company name to the client's name.

```javascript
var company_name = "Looping.Tech";
```

- Change the file **favicon.png** to the client's favicon image in the `/images` folder.

- *(Optional)* Change the company introduction in the **Paragraphs** section in `index.html`:
```html
<h3>Paragraphs</h3>
<p><span class="company_name">[Brand.Name]</span> is a digital agency that provides business strategy and consulting, brand identity and design, UX research, marketing, technology and hosting services to companies of different sizes and in a diverse range of business areas. Our agency is known for successfully harmonizing user needs and business goals to create human-centered development and industry‐changing digital experiences for our clients. <span class="company_name">[Brand.Name]</span> has offices based in Europe and Asia, and is part of the MNK Tech Company. For more information, please visit: <a href="https://www.looping.tech" target="_blank">Looping.tech</a></p>
```

### 2. Change styles to brand design styles 

In `brandstyles.css`,

### 3. Colors

1. Get the hexadecimal values for the brand colors
2. Inside the boxes, change the hexadecimal values in the paragraphs, like so:

```html
<li class="column">
    <div class="color">
        <p>#000000</p><!-- CHANGE HERE -->
    </div>
</li>
```
3. There are a total of three boxes for the dominant colors and a total of five boxes for the secndary colors. If the brand does not have that many colors, boxes can be removed by adding the **.hidden** class to a box, like so:
```html
<li class="column">
    <div class="color hidden"><!-- CHANGE HERE -->
        <p>#000000</p>
    </div>
</li>
```

### 4. Fonts and Typography
1. Add fonts to font folder
2. Change **@font-face** in `brandstyles.css`
3. Change font and color attributes for **body**, **p**, and all heading (**h1**, **h2**, **h3**, **h4**, **h5**, **h6**) elements in `brandstyles.css`


## Favicon Cheat Sheet.

PNG is the preferred format for favicons, try to get this file format in the following sizes:

| Size          | Name              | Usage                     |
| ------------- | ----------------- | ------------------------- |
| 32 x 32       | favicon-32.png    | Desktop brower standard   |
| 128 x 128     | favicon-128.png   | Chrome web store icon     |
| 152 x 152     | favicon-152.png   | iPad                      |
| 167 x 167     | favicon-167.png   | iPad Retina               |
| 180 x 180     | favicon-180.png   | iPhone Retina             |
| 192 x 192     | favicon-192.png   | Google dev web app        |
| 196 x 196     | favicon-196.png   | Chrome                    |


## Changelog.

### Note
When making changes to `index.html`, save changes and reload the document in the web browser.

#### 2020-06-13
* Initial setup

#### 2020-09-30
* Added Favicon Cheat Sheet