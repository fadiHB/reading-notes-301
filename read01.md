# Responsive Web Design

![GitHub Logo](img01/r2.png)

Responsive web design is about creating web pages that look good on all devices!
A responsive web design will automatically adjust for different screen sizes and viewports.

## What is Responsive Web Design?

Responsive Web Design is about using HTML and CSS to automatically resize, hide, shrink, or enlarge, a website, to make it look good on all devices (desktops, tablets, and phones)

## Responsive vs. Adaptive vs. Mobile

Responsive and adaptive web design are closely related, and often transposed as one in the same.
**Responsive** generally means to react quickly and positively to any change, while **adaptive** means to be easily modified for a new purpose or situation, such as change. With **responsive design websites** continually and fluidly change based on different factors, such as viewport width, while **adaptive websites** are built to a group of preset factors.
A combination of the two is ideal, providing the perfect formula for functional websites. Which term is used specifically doesn’t make a huge difference.
**Mobile**, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users.

Currently the most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way. This solution has the benefits of being all three, responsive, adaptive, and mobile.

## Flexible Layouts

Responsive web design is broken down into three main components:

1. flexible layouts
2. media queries
3. flexible media.

### flexible layouts

is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.
Flexible grids are built using relative length units, most commonly percentages or em units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.

Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches. Reason being, the viewport height and width continually change from device to device. Website layouts need to adapt to this change and fixed values have too many constraints.

The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.

                                target ÷ context = result

after that, we should multiply the result by 100 to get the result at a percentage

                                result * 100 = final-Result %

## media queries

Media queries were built as an extension to media types commonly found when targeting and including styles.
Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.
Being able to apply uniquely targeted styles opens up a world of opportunity and leverage to responsive web design.

### Initializing Media Queries

There are a couple different ways to use media queries, using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML documen

### Logical Operators in Media Queries

Logical operators in media queries help build powerful expressions.
There are three different logical operators available for use within media queries, including and, not, and only.

### Mobile First

One popular technique with using media queries is called mobile first. The mobile first approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.

The operating belief behind mobile first design is that a user on a mobile device, commonly using a smaller viewport, shouldn’t have to load the styles for a desktop computer only to have them over written with mobile styles later. Doing so is a waste of bandwidth. Bandwidth that is precious to any users looking for a snappy website.

The mobile first approach also advocates designing with the constraints of a mobile user in mind. Before too long, the majority of Internet consumption will be done on a mobile device. Plan for them accordingly and develop intrinsic mobile experiences.

### Viewport

Mobile devices generally do a pretty decent job of displaying websites these days. Sometimes they could use a little assistance though, particularly around identifying the viewport size, scale, and resolution of a website. To remedy this, Apple invented the viewport meta tag.

## Flexible Media

The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

One quick way to make media scalable is by using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width.

# SMACSS 

## What is it?

What is SMACSS?
SMACSS stands for Scalable and Modular Architecture for CSS and it has 2 core goals.

* Increase the semantic value of a section of html and content
* Decrease the expectation of a specific html structure

Like Object Oriented CSS, SMACSS is an approach to writing css and html with more emphasis placed on using classes. Unlike OOCSS, it doesn’t suggest using classes for everything. It’s fine with IDs and descendent selectors where appropriate.

At the very core of SMACSS is categorization. By categorizing CSS rules, we begin to see patterns and can define better practices around each of these patterns.

Much like OCCSS, the purpose of this categorization is less code repetition, a more consistent experience, and easier maintenance. Under SMACSS there are 5 general categories of css rules.

* Base — These are your defaults (html, body, h1, ul, etc)
* Layout — These divide the page into major sections
* Module — These are the reusable modular components of a design
* State — These describe how things look when in a particular state (hidden or expanded, active/inactive)
* Theme — These define things like a color scheme or typographic treatment across a site

Most of us tend to mix styles across all of these categories, which creates complexity. If instead, we can understand the differences in these categories and apply some guidelines to each we can simplify our css.

Jonathan offers a naming convention for working with SMACSS, though he’s quick to point out you don’t need to follow his convention. He does feel that having some consistent naming convention is important.

* Base — Nothing needed
* Layout — l- or layout- prefixes
* State — is- prefix as in is-active or is-hidden
* Module — Modules just use module name ( .callout ) instead of trying to prefix each, * however related modules receive a consistent prefix to help organize them