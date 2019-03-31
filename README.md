# Scrolling panels example

This is an example of one way to get a layout with a fixed header and any number of independently scrollable columns below it.  The outer columns are fixed width and the center column will stretch to fit the remaining space.

## WebKit scrollbar styling

On WebKit browsers the two right sections have styled scrollbars similar to the Gmail app, with rectangular thumbbars and semi-transparent greyscale colors to overlay the base color of the element.  The left column has a default scrollbar which (on WebKit at least) is opaque white and greys that make it less obvious that it goes with the content to its left.

## Inertia

On WebKit browsers on touchscreen devices, inertia is added to the scrolling.  This is handy and expected effect on iOS devices with Safari and Chrome browsers, for example.