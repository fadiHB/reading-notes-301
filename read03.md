# Javascript Templating

![GitHub Logo](img03/r31.png)

Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.
The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.

**Mustache** is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.
It is often referred to as “logic-less” because there are no if statements, else clauses, or for loops. Instead, there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.

**mustache.js** is an implementation of the mustache template system in JavaScript. It is often considered the base for JavaScript templating. And, since mustache supports various languages, we don’t need a separate templating system on the server side.

# Flexbox

The Flexbox Layout (Flexible Box) module (a W3C Candidate Recommendation as of October 2017) aims at providing a more efficient way to lay out, align and distribute space among items in a container, even when their size is unknown and/or dynamic (thus the word “flex”).

The main idea behind the flex layout is to give the container the ability to alter its items’ width/height (and order) to best fill the available space (mostly to accommodate to all kind of display devices and screen sizes). A flex container expands items to fill available free space or shrinks them to prevent overflow.

## Properties for the Parent (flex container)

### display

This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.

                                        .container {
                                        display: flex; /* or inline-flex */
                                        }

Note that CSS columns have no effect on a flex container.

### flex-direction

This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns.

                        .container {
                        flex-direction: row | row-reverse | column | column-reverse;
                        }

* row (default): left to right in ltr; right to left in rtl
* row-reverse: right to left in ltr; left to right in rtl
* column: same as row but top to bottom
* column-reverse: same as row-reverse but bottom to top

### flex-wrap

two rows of boxes, the first wrapping down onto the second
By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.

                                    .container {
                                    flex-wrap: nowrap | wrap | wrap-reverse;
                                    }

* nowrap (default): all flex items will be on one line
* wrap: flex items will wrap onto multiple lines, from top to bottom.
* wrap-reverse: flex items will wrap onto multiple lines from bottom to top.

## Properties for the Children (flex items)

### order

Diagram showing flexbox order. A container with the items being 1 1 1 2 3, -1 1 2 5, and 2 2 99.

By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container.

                        .item {
                        order: 5; /* default is 0 */
                        }

### flex-grow

two rows of items, the first has all equally-sized items with equal flex-grow numbers, the second with the center item at twice the width because its value is 2 instead of 1.

This defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up.

If all items have flex-grow set to 1, the remaining space in the container will be distributed equally to all children. If one of the children has a value of 2, the remaining space would take up twice as much space as the others (or it will try to, at least).

                                        .item {
                                        flex-grow: 4; /* default 0 */
                                        }
Negative numbers are invalid.

### flex-shrink

This defines the ability for a flex item to shrink if necessary.

                            .item {
                            flex-shrink: 3; /* default 1 */
                            }
Negative numbers are invalid.