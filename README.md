# Scrolling panels example

This is an example of one way to get a layout with a fixed header and any number of independently scrollable columns below it.  The outer columns are fixed width and the center column will stretch to fit the remaining space.

## WebKit scrollbar styling

On WebKit browsers the two right sections have styled scrollbars similar to the Gmail app, with rectangular thumbbars and semi-transparent greyscale colors to overlay the base color of the element.  The left column has a default scrollbar which (on WebKit at least) is opaque white and greys that make it less obvious that it goes with the content to its left.

## Inertia

On WebKit browsers on touchscreen devices, inertia is added to the scrolling.  This is handy and expected effect on iOS devices with Safari and Chrome browsers, for example.

## TO-DO

- Fix issues on iOS devices with Safari

  The browser URL bar and footer hide part of the page and make the whole page scrollable since it no longer fits in the leftover space, but apparently thinks the viewport is the full screen height.  The browser bar and footer won't go away either since you can't really scroll the page down.

  Chrome on iOS also shows the URL bar and footer, but resizes the viewport to the leftover space between them, so everything works correctly.

  There seem to be two possible solutions:

  - Make sure the viewport size (or whatever the CSS code is using to size the container) matches the space that is actually available between the URL bar and footer.
  - Make the URL bar and footer hide so the page has the full screen.