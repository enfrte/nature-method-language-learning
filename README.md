# nature-method-language-learning

Create digital versions of the old books based on the nature method of language learning. 

## Requirements

AlpineJS 3x - https://alpinejs.dev/

File path: /js/alpine-js-3x.js

## JSON naming conventions and behaviour

Pages from the printed book are mapped to "pages". In the html markup, "pages" are assigned the article tag. 

Each chapter has a title. Chapter ("chapter_title") titles always appear before the content on a new page. However, other (sub) titles can appear in the chapter and can be added to the content with header tag markup.

Titles can appear mid page or even twice in the same page (possibly). Therefore they are added to the content in the order they appear in the text. They also get a 'page-title' CSS class. Same deal with asides, which gets an 'aside-title' CSS class.

"content" is divided by sentence. The book adds horizintal padding between sentences to help the user focus, so this helps with styling. Same deal with asides. 

There can be more than one aside on the page. To help with styling, each is separated with their own array block. 

pages.id = the page number in the book. 

