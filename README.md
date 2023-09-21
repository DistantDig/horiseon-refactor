# Horiseon-Refactor

## Description 

This repository was designed to refactor previously existing code to be cleaner and more organized without changing the function or the user's view of the page. This refactor cleans up the code for the (Fictional) company of Horiseon. The point of this project was to exercise fundamental html and css concepts by searching for and correcting any mistakes in the source code.


## The User Story

```
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines
```


## The Acceptance Criteria

```
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the icon and image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title
```

## Changes To Meet The Acceptance Criteria 

### Semantic HTML Elements

At the start of the project, the majority of the code was sectioned with only <div> elements. I instead went through and renamed all of these elements to reflect the code contained within. With this I also created more spacing within the code for easier readability, although this may simply be a personal preference.

```html
    <section class="search-engine-optimization">
        <img src="./assets/images/search-engine-optimization.jpg" alt="Notepad on a desk" class="float-left" />
        <h2>Search Engine Optimization</h2>
        <p>
            The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
        </p>
    </section>

    <section id="online-reputation-management" class="online-reputation-management">
        <img src="./assets/images/online-reputation-management.jpg" alt="Laptop displaying reputation graph" class="float-right" />
        <h2>Online Reputation Management</h2>
        <p>
            The web is full of opinions, and some of these can be negative. Social media allows anyone with an internet connection to say whatever they want about your business. Online Reputation Management gives you the control over what potential customers see when they search for your business.
        </p>
    </section>
```

### Logical Structure

I created spacing for the HTML page for easier readability as well as organized the CSS file into categories that I thought would make sense. I also added comments to label these categories, and organized them in a similar flow to the HTML file.

```css
/* Main */

.content {
    width: 75%;
    display: inline-block;
    margin-left: 20px;
}

.search-engine-optimization h2,
.online-reputation-management h2,
.social-media-marketing h2 {
    margin-bottom: 20px;
    font-size: 36px;
}
```


### Accessible Alt Attributes

Each image seemed to be missing an alt attribute, and so I went through and provided a short description to serve as one. This would include each major image as well as shorter icons found on the page.

```html
<img src="./assets/images/search-engine-optimization.jpg" alt="Notepad on a desk" class="float-left" />
```

### Headers In Sequential Order

The header elements seemed to be mostly in a fitting order throughout the document, but I did find it odd that the footer's header was using an h2 element. I instead changed it to use h4, and ensured that the text remained the same size through the CSS file.

```html
<h4>Made with ❤️️ by Horiseon</h4>
```
```css
.footer h4 {
    font-size: 20px;
}
```