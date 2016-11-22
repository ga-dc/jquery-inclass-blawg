# My Blawg: JS Selectors Practice

Open the included `index.html` in your browser.

# Part One: Vanilla JS

Write down how you would select the following DOM objects on "My Blawg". Use only the following methods or attributes:

- `querySelector`
- `querySelectorAll`
- `getElementById`
- `innerHTML`

---

1. The first `<a>` element on the page
document.querySelector("a");

- All `<a>` elements on the page
- document.querySelectorAll("a");
-
- Using its ID, the `<h1>` at the top of the page
- document.getElementById("h1");
-
- All elements with class `post`
- document.querySelectorAll(".post");
-
- The first element with class `post`
- document.querySelector(".post");
-
- The second element with class `post`
document.querySelectorAll('.post')[1]
-
- The HTML content of the first `<p>` element on the page
document.getElementById("p").innerHTML;

Try it Yourself »
# Part Two: jQuery

First, use a `<script>` tag in `index.html` to include the minified jQuery file in the `js` folder.

Then, write down how you would select the following DOM objects on "My Blawg". Use only the following methods or attributes:

- `$`
- `eq`
- `html`

---

1. All `<a>` elements on the page
2. $('a')
3.
- The first `<a>` element on the page
- $('a:first-of-type')
-
- Using an ID, the `<h1>` at the top of the page


- All elements with class `post`
- $('.post')
-
- The first element with class `post`
- $('.post:first-of-type')
-
- The second element with class `post`
- $('.post:nth-of-type(1)')
-
- The HTML content of the first `<a>` element on the page
$('a:first-of-type').html

Bonus:
- Using a CSS pseudo-selector, the third element with class `post`
$('.post:nth-of-type(2)')

- Using one of its HTML attributes, the fourth `<img>` on the page
$('img:nth-of-type(3)')

# Part Three: Getting and Setting

Using these jQuery methods or attributes, follow the instructions below:

- `$`
- `eq`
- `html`
- `css`
- `prop`

Things to consider:
- What's the difference between `$("body").html()` and `$("body").html("hello")`?
- `$("p")` selects all `<p>` elements on the page.
  - If you run `$("p").html()`, how many elements' HTML does it return?
  - If you run `$("p").html('hello')`, how many elements does it affect?
  - What about the other methods?

---out of time :-(

1. Get the HTML content of the second `<p>` element on the page
2. $('p:nth-of-type(1)').html()
3. 
- Set the HTML content of the second `<p>` to something else weird
- Get the background color of the body
- Set the background color of the body to "burlywood"
- Get the `alt` value of the fourth `<img>` on the page
- Set the `alt` value of the fourth `<img>` on the page to "Why is my boat upside down?"
