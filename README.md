# Web_Development_Front_End

# -----------------------------------------------------------------------------------------------------------------------------------------------------------------

# Learn
-> Learn to explain what web development is and the roles of HTML, CSS, and JavaScript in creating web content.

# What is web development?
-> Web development is a specific field of software engineering that focuses on building web pages. Web pages, or web apps, are codebases that are downloaded and run in our web browser (e.g., Google Chrome) each time a user navigates to the website address. This differs from other software which is usually downloaded once and run as a standalone application on your computer or phone. 
-> Web development makes for an exciting career, as a web development cycle is usually much shorter and you get to iterate over your software at a much faster rate.
The major building blocks of the web are HTML, CSS, and JavaScript. We will be talking about all three languages. We can also think of web development as being split into two main categories: front end and back end. We will discuss what each entails.

# What is meant by the term front end?
-> Everything you have ever seen on the web is considered ‘front end’. Front end is what we see when we open a web page or app. Code is downloaded from a server and is rendered to the screen by a web browser. What happens when we interact with the code is also considered front end. This is often referred to as the ‘Presentation Layer’ or ‘Client’ in software development terms.
-> The front end is built out of three languages: HTML, CSS, and JavaScript. HTML allows us to put content on our page: text, headers, images, buttons, links, and etc. CSS is used to style our page. It allows the contents to have different text colors, background colors, as well as dealing with the positioning of the content on the page. 
-> JavaScript makes our page dynamic. It allows for the content to change on a mouse hover or click and also lets us submit data and have data rendered on our page (such as submitting a new blog post or having your feed populated when you open Facebook).

# What is a framework?
-> Real world web development relies heavily on the use of frameworks. Frameworks aren’t exactly new languages, but are more like add-ons to existing languages. These frameworks slightly change the rules and syntax of a language, but save us a lot of time and effort in writing web development code.
-> For example, a CSS framework like Bootstrap will require us to write our CSS using slightly different rules than regular (vanilla) CSS. It will also limit the level of customization we can do using CSS. But the drawbacks are often worth it, because Bootstrap makes styling our sites far easier and allows us to create mobile-friendly pages with minimal effort.

# -----------------------------------------------------------------------------------------------------------------------------------------------------------------

# Learn to use HTML code to create a basic webpage.

# What is HTML?
-> As already mentioned, HTML (which stands for Hyper Text Markup Language) is one of the languages we use for web development. HTML was created as a language when the first visual web browsers came into existence in the early 90s. It is read by the browser and then used as a blueprint for displaying information on your screen.
-> HTML is not considered a “programming language”, but is rather what we call a “markup language”. This means that it is specifically designed to render data in a graphical form (rather than execute tasks).

# Anatomy of an HTML document.
The main parts of our element are as follows:

# The opening tag: 
-> This consists of the name of the element (in this case, p), wrapped in opening and closing angle brackets. This states where the element begins or starts to take effect — in this case where the paragraph begins.

# The closing tag: 
-> This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends — in this case where the paragraph ends. Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.

# The content: 
-> This is the content of the element, which in this case, is just text.

# The element: 
-> The opening tag, the closing tag, and the content together comprise the element.

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="My test image">
  </body>
</html>

# <!DOCTYPE html> — doctype. 
-> It is a required preamble. In the mists of time, when HTML was young (around 1991/92), doctypes were meant to act as links to a set of rules that the HTML page had to follow to be considered good HTML, which could mean automatic error checking and other useful things. However these days, they don't do much and are basically just needed to make sure your document behaves correctly. That's all you need to know for now.

# <html></html> — the <html> element. 
-> This element wraps all the content on the entire page and is sometimes known as the root element.

# <head></head> — the <head> element. 
-> This element acts as a container for all the stuff you want to include on the HTML page that isn't the content you are showing to your page's viewers. This includes things like keywords and a page description that you want to appear in search results, CSS to style our content, character set declarations, and more.

# <meta charset="utf-8">.
  This element sets the character set your document should use to UTF-8 which includes most characters from the vast majority of written languages. Essentially, it can now handle any textual content you might put on it. There is no reason not to set this and it can help avoid some problems later on.

# <title></title> — the <title> element. 
-> This sets the title of your page, which is the title that appears in the browser tab the page is loaded in. It is also used to describe the page when you bookmark/favorite it.

# <body></body> — the <body> element. 
-> This contains all the content that you want to show to web users when they visit your page, whether that's text, images, videos, games, playable audio tracks, or whatever else.

# Headings:
-> Heading elements allow you to specify that certain parts of your content are headings — or subheadings. In the same way that a book has the main title, chapter titles, and subtitles, an HTML document can too. HTML contains 6 heading levels, <h1>–<h6>, although you'll commonly only use 3 to 4 at most:

<h1>My main title</h1>
<h2>My top level heading</h2>
<h3>My subheading</h3>
<h4>My sub-subheading</h4>

# Paragraphs:
-> As explained above, <p> elements are for containing paragraphs of text; you'll use these frequently when marking up regular text content:
  
  <p>This is a single paragraph</p>
  
# Lists:
-> A lot of the web's content is lists and HTML has special elements for these. Marking up lists always consists of at least 2 elements. The most common list types are ordered and unordered lists:

# Unordered lists:
-> They are for lists where the order of the items doesn't matter, such as a shopping list. These are wrapped in a <ul> element.

# Ordered lists:
-> They are for lists where the order of the items does matter, such as a recipe. These are wrapped in an <ol> element.
Each item inside the lists is put inside an <li> (list item) element.
  
  <p>At Mozilla, we’re a global community of</p>

<ul>
  <li>technologists</li>
  <li>thinkers</li>
  <li>builders</li>
</ul>

<p>working together ... </p>

# Links:
-> Links are very important — they are what makes the web a web! To add a link, we need to use a simple element — <a> — "a" being the short form for "anchor". To make text within your paragraph into a link, follow these steps:
  
  <a>Mozilla Manifesto</a>
  <a href="">Mozilla Manifesto</a>
  <a href="https://www.mozilla.org/en-US/about/manifesto/">Mozilla Manifesto</a>
  
-> You might get unexpected results if you omit the https:// or http:// part, called the protocol, at the beginning of the web address.

# -----------------------------------------------------------------------------------------------------------------------------------------------------------------

# What is CSS?
-> Like HTML, CSS is not a programming language. It's not a markup language either. CSS is a style sheet language. CSS is what you use to selectively style HTML elements. For example, this CSS selects paragraph text, setting the color to red:

 p {
  color: red;
}

# Anatomy of a CSS ruleset:

# Selector:
-> This is the HTML element name at the start of the ruleset. It defines the element(s) to be styled (in this example, <p> elements). To style a different element, change the selector.

# Declaration:
-> This is a single rule like color: red;. It specifies which of the element's properties you want to style.

# Properties:
-> These are ways in which you can style an HTML element. (In this example, color is a property of the <p> elements.) In CSS, you choose which properties you want to affect in the rule.

# Property value:
-> To the right of the property—after the colon—there is the property value. This chooses one out of many possible appearances for a given property. (For example, there are many color values in addition to red.)

-> Apart from the selector, each ruleset must be wrapped in curly braces. ({})
-> Within each declaration, you must use a colon (:) to separate the property from its value or values.
-> Within each ruleset, you must use a semicolon (;) to separate each declaration from the next one.

eg:
p {
  color: red;
  width: 500px;
  border: 1px solid black;
}

# Selecting multiple elements:
-> You can also select multiple elements and apply a single ruleset to all of them. Separate multiple selectors by commas:

p, li, h1 {
  color: red;
}

# Fonts and text :
-> First, find the output from Google Fonts that you previously saved from What will your website look like?. Add the <link> element somewhere inside your index.html's head (anywhere between the <head> and </head> tags).
-> Add the following lines (shown below), replacing the font-family assignment with your font-family selection from What will your website look like?. The property font-family refers to the font(s) you want to use for text. This rule defines a global base font and font size for the whole page. Since <html> is the parent element of the whole page, all elements inside it inherit the same font-size and font-family.
  
eg:
<link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
html {
  font-size: 10px; /* px means "pixels": the base font size is now 10 pixels high  */
  font-family: "Open Sans", sans-serif; /* this should be the rest of the output you got from Google fonts */
  
-> Now let's set font sizes for elements that will have text inside the HTML body (<h1>, <li>, and <p>). We'll also center the heading. Finally, let's expand the second ruleset (below) with settings for line height and letter spacing to make body content more readable.
  
  eg:
  h1 {
  font-size: 60px;
  text-align: center;
}

p, li {
  font-size: 16px;
  line-height: 2;
  letter-spacing: 1px;
}

# CSS layout is mostly based on the box model:

# Padding:
-> The space around the content. In the example below, it is the space around the paragraph text.

# Border: 
-> The solid line that is just outside the padding.

# Margin: 
-> The space around the outside of the border.

# width (of an element).

# Background-color:
-> The color behind an element's content and padding.

# Color: 
-> The color of an element's content (usually text).

# Text-shadow: 
-> Sets a drop shadow on the text inside an element.

# Display: 
-> Sets the display mode of an element. (keep reading to learn more)

# Changing the page color:
html {
  background-color: #00539F;
}

# Styling the body:
body {
  width: 600px;
  margin: 0 auto;
  background-color: #FF9500;
  padding: 0 20px 20px 20px;
  border: 5px solid black;
}

# Positioning and styling the main page title:
h1 {
  margin: 0;
  padding: 20px 0;
  color: #00539F;
  text-shadow: 3px 3px 1px black;
}

-> Text-shadow applies a shadow to the text content of the element. 
Its four values are:
-> The first pixel value sets the horizontal offset of the shadow from the text: how far it moves across.
-> The second pixel value sets the vertical offset of the shadow from the text: how far it moves down.
-> The third pixel value sets the blur radius of the shadow. A larger value produces a more fuzzy-looking shadow.
-> The fourth value sets the base color of the shadow.

# Centering the image:
img {
  display: block;
  margin: 0 auto;
}

# -----------------------------------------------------------------------------------------------------------------------------------------------------------------


