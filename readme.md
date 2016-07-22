# Introduction to SASS

## Problems with CSS

* Does not scale to large web sites / applications
    - Does not provide any mechanisms for reuse.
* Cascading not a good fit for component based development
    - Cascading is better fit for publishing static content
    - Components are reusable and should not radically change appearance based on context
* Organization: How to organize and manage the following responsibilities:
    - Simple styling: colors, fonts, borders, shadows
    - Layout: margins, padding, justification, alignment, grid systems
    - States: enabled, disabled, visible, hidden
    - Animations
* Naming - class names
    - How to avoid name conflicts
    - How to be semantic

## What are Preprocessors?

* Preprocessors allow us to write source code in one language and translate
  the source code into another language.

* Sometimes preprocessors don't translate from one language to another but
  do apply values to placeholders (i.e. templates).

### Examples:

* `ERB`: evaluate Ruby expressions in an `HTML`, `CSS`, or other source file.
* `SLIM`: translate `SLIM` files into `HTML`.
* `CoffeeScript`: compile CoffeeScript source code into `JavaScript`.
* `SASS`: compile `SASS` source code into `CSS` source code.
* `LESS`: compile `LESS` source code into `CSS` source code.

## Advantages of Preprocessing?

Sometimes we cannot alter the target language of an execution environment
(such as a browser), but we want to write our source code in something other
than what the target execution environment supports.

* `SLIM` instead of `HTML`
* `CoffeeScript` instead of `JavaScript`
* `SASS` instead of `CSS`

Thus we can use advanced features of a new language without waiting for the
browser to support these advanced features.

We can also more easily support browser quirks and idiosyncrasies by handling
them in the preprocessor instead of in the original source code.


## What is SASS?

* `SASS` is an extension of CSS.
* `SASS` adds the following features to CSS:
  - nesting              makes code easier to read and maintain - try it at `http://css2sass.herokuapp.com/`
  - variables            DRY up with reusable expressions
  - operators            FLEXIBLE via math calculations
  - partials & imports   ORGANIZE by splitting your CSS up into separate files that get combined later
  - functions            DRY up with reusable chunks of logic
  - mixins               DRY up with reusable chunks of SCSS
  - extends              DRY up by extending a base class

* See: [Sass Basics](http://sass-lang.com/guide)

## Advantages of Using SASS

* DRY up your CSS via `variables`, `functions`, `mixins`, and `extends`
* Organize your CSS via `nesting` and `partials`
* Use math expressions in your CSS via `operators`
* Optimize the CSS output: SASS only includes what is used in your SASS files.

For a real-time preview, see: [SASSmeister](http://sassmeister.com/).

## Lab

The starter for this lab is at [SASS Lab 1 Starter](http://codepen.io/drmikeh/pen/empbzO)
The completed lab is at [SASS Lab 1 Finished](http://codepen.io/drmikeh/pen/wBKRxN)

Given a div container that has 3 child divs:

    <body>
      <div class="container">Colors
        <div class="red">  <p>Red</p></div>
        <div class="green"><p>Green</p></div>
        <div class="blue"> <p>Blue</p></div>
      </div>
    </body>

Using only vanilla CSS (no SASS, no Bootstrap, no Foundation) style the above HTML as follows:

* The outer div has:
    - a width of 400px
    - a height of 200px
    - background color of light gray
    - a border of black,
    - a border radius of 20px
    - and a label of “Colors” near the top of the div

* The inner divs should fit nicely inside the outer div and have the following:
    - Background colors of “##FFB3B3”, “light green”, and “light blue”, respectively.
    - Borders of red, green, and blue, respectively.
    - Labels of “Red”, “Green”, and “Blue”, respectively.
    - A border radius of 10px.

* Now convert the CSS to SASS and make it as DRY as possible. Feel free to use the Compass SASS library.
* Bonus:
    - Make it easy to resize the outer div and have the inner div’s resized accordingly (don’t use percentages).
    - Make the labels in the color divs have a text color that is the complement of the background color.


## Resources

* [SASSmeister](http://sassmeister.com/)
* [CSS 2 SASS Online Converter](http://css2sass.herokuapp.com/)
* [SMACSS](https://smacss.com) - Scalable and Modular Architecture for CSS
* [OOCSS](http://oocss.org)    - Object Oriented CSS
* [BEM](https://bem.info)      - Block, Element, Modifier
* [SASS](http://sass-lang.com) - Preprocessor
* [LESS](http://lesscss.org)   - Preprocessor
* [Bourbon](http://bourbon.io) - Bourbon SASS Library
* [How to make your CSS awesome with Bourbon, Neat, Bitters and Refills!](https://www.youtube.com/watch?v=8ItNE_DX6Cc)
* [OOCSS and SMACSS](http://www.slideshare.net/maxdesign/css-oocss-and-smacss)
* [Organizing CSS, OOCSS, SMACSS, and BEM](http://mattstauffer.co/blog/organizing-css-oocss-smacss-and-bem)
