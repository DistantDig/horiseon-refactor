# Horiseon-Refactor

## Description 

This repository was designed to refactor previously existing code to be cleaner and more orginized without changing the function or the user's view of the page. This refactor cleans up the code for the (Fictional) company of Horiseon. The point of this project was to excercise fundamental html and css concepts by searching for and correcting any mistakes in the source code.


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

### Semantic HTML Elemnts

At the start of the porject, the majority of the code was sectioned with only &ltdiv$gt elements. I instead went through and renamed all of these elements to reflect the code contained within. With this I also created more spacing within the code for easier readability, although this may simply be a personal preferance.

```html
        <section class="search-engine-optimization">
            <img src="./assets/images/search-engine-optimization.jpg" alt="Notepad on a desk" class="float-left" />
            <h2>Search Engine Optimization</h2>
            <p>
                The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
            </p>
        </section>
```