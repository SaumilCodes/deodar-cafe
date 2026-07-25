# Deodar Cafe

A website for a small fictional cafe in Waknaghat, Himachal Pradesh, the town where my university is. Four pages, one stylesheet, no JavaScript and no frameworks.

I built this after finishing Meta's Introduction to Front-End Development and HTML and CSS in Depth courses on Coursera, to use as much of them as I could in one project. It has since been rebuilt once, with a warmer palette, a serif for the headings and a few features I wanted to try without reaching for JavaScript.

## Things worth pointing at

- **Menu filter.** The chips at the top of the menu page hide and show categories. Five radio buttons, and CSS picks what stays visible with `#cat-chai:checked ~ .menu-body .menu-section:not(.is-chai) { display: none; }`.
- **Lightbox.** Clicking a drawing on the About page opens it full size. Each overlay has an id, and `.lightbox:target` shows the one whose id is in the address bar. Closing it is just a link back to `#gallery`.
- **FAQ.** Plain `details` and `summary`, with the marker swapped for a plus that rotates into a cross.
- **Booking form.** Fieldsets, a phone pattern, date and time inputs, and validation colours that only appear after you have touched a field, using `:user-valid` and `:user-invalid`.
- **Scrolling notice band** on the home page, two copies of the same line sliding left, paused on hover.
- **Dark mode** that follows the device, and reduced motion turns the animations off.

All the food drawings are SVGs I made for this project, including the little map on the home page.

Live at [saumilcodes.github.io/deodar-cafe](https://saumilcodes.github.io/deodar-cafe/)

## Pages

- `index.html` home
- `menu.html` the full menu
- `about.html` story, house rules and the gallery
- `book.html` booking form and FAQ

## Running it

No build step. Clone and open `index.html` in a browser.
