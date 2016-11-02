# Exam: HTML & CSS

### Getting Started
 - Fork this repository under your own account
 - Commit your progress frequently and with descriptive commit messages
 - All your answers and solutions should go in this repository

### What can I use?
 - You can use any resource online, but **please work individually**
 - Instead of copy-pasting your answers and solutions, write them in your own words.


# Tasks

## 1. Build a design (~90 minutes) [10 points]
Build the following profile cards according to the design provided.   
Follow the design as closely as possible.   
Commit an HTML and a CSS file to this repository.
![design](exercise-1.png)

### Assets
John Duck | Jane Duck | Pencil icon
--------- | --------- | -----------
![duck](duck.jpg) | ![duck](duck2.jpg) | ![pencil-icon](edit-icon.png)   

### Other data
  - Name font size: 28 pixels
  - Text size: 14 pixels
  - Font family: Arial, sans-serif

### Acceptance criteria
The task is accepted if:
  - The result follows design [2p]
  - The code follows style guide [1p]
  - The CSS & HTML are valid [1p]
  - The HTML considers semantic responsibilities [2p]
  - The code avoids code duplication [2p]
  - The CSS has meaningful and short selectors [2p]

Extra points for if:
  - the result is centered on the page [2p]


## 2. Understand code (~15 minutes) [2 points]
Read the following code snippet:   
What is the distance between the top-left corner of the document body and the yellow box?   
Give a detailed explanation below!   
Add your answer to this readme file, commit your changes to this repository.
```HTML
<!DOCTYPE html>
<html>
  <head>
    <style>
      body {
        padding: 0px;
        margin: 0px;
      }
      .foo {
        top: 20px;
        left: 20px;
        width: 100px;
        height: 100px;
        position: absolute;
        background: blue;
      }
      .bar {
        top: 20px;
        left: 20px;
        width: 30px;
        height: 30px;
        position: absolute;
        background: yellow;
      }
    </style>
  </head>
  <body>
    <div class="foo">
      <div class="bar"></div>
    </div>
  </body>
</html>
```

> The distance between the yellow box and the top-left corner of the document body is 40px. The body has zero margin, and the blue square's position is set to absolute, which means it is positioned to the top-left corner of the closest parent that is also positioned (in this case, it is the document body itself). The yellow box is inside the blue square, and also absolute positioned. In this case, it means that it is 20px away from the closest positioned parent's top-left corner, which is the blue square. The two positon values add up to 40px.

#### Your answer: [2p]

## 3. Explain concepts (~15 minutes) [4 points]
Add your answer to this readme file, commit your changes to this repository.


### Explain the difference between `display: block` and `display: inline` in CSS! What is `display: inline-block`?

>The "display:block" value is the default behavior of the elements of a CSS. It means that it will always position itself into a separate line, regardless of the surrounding content. The value "display:inline" stands for elements that positon themselves one after the other in the same line, allowing every following inline element to fill the available space. The value "display:inline-block" works much like float did, before the flexbox layout model was introduced. It means that the inline-block element will position itself into a separate line, but allows the surrounding content to flow around it, as if it was a floated element.

#### Your answer: [2p]


### What is the difference between a `<section>` and an `<article>` element? Name one good example of using an `<article>`.

>The section and the article are both semantic html elements. They both mark a standalone part of the whole content and they typically begin with a heading. The article is more often used for news articles, blog notes and such. The section can either define a larger or a smaller portion than the article, that usually depends on the type of the content. The article can contain a section and a section can contain an article, all that matters is that it is consistently used throughout the html.

#### Your answer: [2p]
