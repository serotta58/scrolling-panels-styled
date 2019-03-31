# Scrolling panels example

This is an example of one way to get a layout with a fixed header and any number of independently scrollable columns below it.  The outer columns are fixed width and the center column will stretch to fit the remaining space.

## WebKit scrollbar styling

On WebKit browsers the two right sections have styled scrollbars similar to the Gmail app, with rectangular thumbbars and semi-transparent greyscale colors to overlay the base color of the element.  The left column has a default scrollbar which (on WebKit at least) is opaque white and greys that make it less obvious that it goes with the content to its left.

## Inertia

On WebKit browsers on touchscreen devices, inertia is added to the scrolling.  This is handy and expected effect on iOS devices with Safari and Chrome browsers, for example.

## To-Do

- Fix iPhone/Safari issue that makes whole page scrollable when it shouldn't be

  On an iPhone SE in landscape mode, the browser URL bar and footer hides part of the page.  This makes the whole page scrollable since it no longer fits in the leftover space.  The browser URL bar and footer won't go away either since you can't really scroll the page down past viewport size.  On other pages that are typically longer, the URL bar and footer shrink when you scroll the page away from the top.

  This is not an issue with Chrome on the iPhone.

- iOS URL bar and footer won't shrink or hide

  Typically, pages are longer than the viewport, and scrolling down causes the iOS Safari and Chrome browsers to shrink or hide the URL bar and footer.  But since this page keeps everything within the viewport, this feature of the browser is never triggered, resulting in less real estate for the page.

  Find a way to minimize or close the URL bar and footer.  And figure out how to bring them back when needed, such as to enter something into the URL input.

  This is primarily an issue for phones where the browser takes up a larger percentage of the space.