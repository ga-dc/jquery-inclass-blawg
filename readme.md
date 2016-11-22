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

document.querySelector('a');


- All `<a>` elements on the page

document.querySelectorAll('a');


- Using its ID, the `<h1>` at the top of the page

document.getElementById("logo");


- All elements with class `post`

document.querySelectorAll(".post");


- The first element with class `post`

document.querySelector(".post");


- The second element with class `post`

document.querySelectorAll(".post")[1];


- The HTML content of the first `<p>` element on the page

document.querySelector('a').innerHTML


# Part Two: jQuery

First, use a `<script>` tag in `index.html` to include the minified jQuery file in the `js` folder.

Then, write down how you would select the following DOM objects on "My Blawg". Use only the following methods or attributes:

- `$`
- `eq`
- `html`

---

1. All `<a>` elements on the page

$('a')


- The first `<a>` element on the page

$('a:first')


- Using an ID, the `<h1>` at the top of the page

$("#logo")


- All elements with class `post`

$(".post")


- The first element with class `post`

$(".post:first")


- The second element with class `post`

$(".post").eq(1)


- The HTML content of the first `<a>` element on the page

$('a:first').html()


Bonus:
- Using a CSS pseudo-selector, the third element with class `post`

$(".post").eq(2)
$(".post:contains('Second')")


- Using one of its HTML attributes, the fourth `<img>` on the page

$("[alt='balloons']")

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

---

1. Get the HTML content of the second `<p>` element on the page

$("p").eq(1).html();


- Set the HTML content of the second `<p>` to something else weird

$("p").eq(1).html("Frosty the snowman was a happy jolly soul");


- Get the background color of the body

$("body").css("background-color")


- Set the background color of the body to "burlywood"

$("body").css("background-color","burlywood")


- Get the `alt` value of the fourth `<img>` on the page

$("img").eq(3).attr("alt")


- Set the `alt` value of the fourth `<img>` on the page to "Why is my boat upside down?"

$("img").eq(3).attr("alt","Why is my boat upside down?")
