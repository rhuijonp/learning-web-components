# Exercises

## Excercise 1
Use selectors to fix the styling in the following code pen:

```
<div class="container">
  <h1></h1>
  <main id="content">
    <h1>My List of Favorite Animals</h1>
    <ul>
      <li class="animal favorite">Kangaroo</li>
      <li class="animal">Puffer</li>
      <li class="animal">Meadowlark</li>
      <li class="animal">Walrus</li>
      <li class="animal">Armadillo</li>
    </ul>
  </main>
  <div class="favorites">
    <h2>Other Favorites</h2>
    <p class="food">I also really enjoy sushi.</p>
    <p class="sport">My family enjoys soccer, but I don't normally enjoy sports.</p>
  </div>
</div>

***************************************************************

body {
  padding: 2% 5%;
  color: #555;
}

/* Write your CSS Styles below: */

ul {
  color: red;
}

.favorites {
  background-color: yellow;
}

.food {
  color: green;
}


```
See result [here](codepen_e1.jpg).

## Exercise 2

1. Determine the color of the p element using the information below:

The p element is located on line 30.

An HTML document has three external stylesheets attached, and a style tag defined within the body.

* Two of the external stylesheets are located at line 8 and 9, within the head tag.
* The final external stylesheet is located at line 64, before the end of the body tag (line 65 is ““)
* The style tag is defined on line 24, with its closing tag on line 29.

The stylesheet on line 8 has the ruleset: p {color: green;}.
The stylesheet on line 9 has the ruleset: p {color: yellow;}.
The stylesheet on line 64 has the ruleset: p {color: cyan;}.
The style tag on line 24 has the ruleset: p {color: orange;}.

Use the rules of how styles are applied to determine the color that the p element will have.

Answer: **Orange**, because the innermost is the inline style that applies.

## Exercise 3
Use your newfound knowledge of combinators for the following exercises. Do the exercises in this codepen.2

1. In a new ruleset, use a combinator to color all .b elements that are siblings of a a element.
1. Use a selector with a combinator to color all siblings of .c orange.
1. Use a selector with a combinator to color all immediate descendants of elements with the class name animals green.

See results [here](codepen_e3.jpg)

## Exercise 4
1. Write a CSS class that will italicize, uppercase, and strike-through its text.
	```
.italicUpperCaseStrike {
	font-style: italic;
	text-transform: uppercase;
	text-decoration: line-through;
	}
	
	```
2. Navigate to Google’s Library of web fonts: www.google.com/fonts; then, choose a font you find pleasing. Write the CSS class named myfont that changes the font family to your chosen font, falling back to the fonts Lora and Times New Roman, and finally falling back one more time to a generic font family of your choosing.

```
/* This did not work

@font-face {
	font-family: Gaegu;
	src: url('https://fonts.google.com');
}

.myfont {
	font-family: Gaegu, Lora, "New Times Roman", sans;
	font-size: 3em;
}

/* But this did


<link href="https://fonts.googleapis.com/css?family=Gaegu" rel="stylesheet">

<style>
	.myfont {
	font-family: Gaegu;
	font-size: 3.5em;
}

```
See the result [here](FontFace.jpg)

3. Spend time experimenting with the CSS line-height property and create three classes, each corresponding to significantly different line-heights. Which line-height do you find easiest to read?

See [result](LineHeight.jpg)


## Excercise 5

1. Calculate the result in pixels: What is 80% of 16px?
answer: 12.8px

1. Calculate the result in em: What is 2em of 1.6em
answer: 0.4em or 2em > 1.6em by .4em

1. Determine the child‘s font size in the below sample:
```

html {
  font-size: 10px;
}
 
parent {
  font-size: 2em;
}
 
.parent .child {
  font-size: 1.6rem;
}
```
answer: about 16px;

## Exercise 6

1. Create a web page that resembles a newspaper, with a heading area, 
three columns, and a footing area. Each column needs an `<h3>` tags and 
at least 5 `<p>` tags. You will need to utilize floats, percentage 
widths, and clears to succeed.
2. After creating the newspaper layout in the exercise above, write a 
simplified write-up of how floats function as if you were writing it for 
a child. Try to find an analogy or example from the physical world, but 
also try to adhere to accuracy. Add your simplified write-up to the 
center column of your newspaper layout. The write-up should be between 3 
and 5 paragraphs.

See result [here](newspaper.html).
