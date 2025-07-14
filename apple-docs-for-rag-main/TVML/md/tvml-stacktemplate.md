

- TVML
-  stackTemplate 

# stackTemplate

Displays groups of products.

## Overview

Use the `stackTemplate` element to display, for example, displaying different genres of movies. Each group of products is displayed directly underneath the previous group. Products can be displayed in different ways using `carousel`, `grid`, and `shelf` elements. The following figure shows the basic layout for a `stackTemplate` page. The theme for the stack template defaults to the system preference.

### Main Elements

The following listing shows the main elements of the `stackTemplate` element in TVML format.

```

        …

                …

```

Note

The `shelf` element can be replaced with a `grid` or `carousel` element to change the way products are displayed.

#### Element Descriptions

banner  
A page description along the top of the screen.

carousel  
Element that contains all elements used to display groups of products, such as dramas and comedies, in a horizontal format.

collectionList  
Element that contains all elements used to display groups of products, such as dramas and comedies, in a horizontal format.

grid  
Element that contains all elements used to display groups of products, such as dramas and comedies, in a grid format.

lockup  
Element containing `img` and `title` elements used to describe a product.

section  
Element containing a group of `lockup` elements.

shelf  
Element containing a group of `section` elements.

### Example

The following listing shows the TVML for a `stackTemplate` example:

```

            Available Action Movies

                        Movie 1

                        Movie 2

                        Movie 3

                        Movie 4

                        Movie 5

                        Movie 6

```

The following figure shows the output for the above example:

You can also customize the stack template’s background content. To do so, embed a `mediaContent `element in a `background `element, as shown in this example:

```

```

When you add a video in the background, playback starts 5 seconds after the page is loaded. The video does not repeat.

## Topics

### Valid TVML Attributes

binding

Associates information in a data item with an element.

itemID

Mark elements for reuse during DOM updates.

layoutDirection

Specifies the direction in which text is displayed.

needsMoreThreshold

Sets the amount of remaining screen lengths before firing the needs more event.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

## See Also

### Full-Page Templates

alertTemplate

Displays important information to the user.

catalogTemplate

Displays groups of items along one side of a page and images of a group’s contents on the other side.

compilationTemplate

Displays information about a single media item and its components.

descriptiveAlertTemplate

Displays large amounts of important information to the user.

divTemplate

Provides the ability to create pages that don’t conform to a layout defined by another template.

formTemplate

Provides the ability to gather information from the user.

listTemplate

Displays a list of items along one side of a page and the corresponding image on the other side.

loadingTemplate

Displays a spinner and description on the screen.

mainTemplate

Displays user options for a media item.

menuBarTemplate

Creates a page with items along the top and related information below.

oneupTemplate

Creates a page that allows users to navigate between full-screen images.

paradeTemplate

Displays a groups of items along one side of a page and scrolling images on the other side.

productBundleTemplate

Displays information for a group of related media items.

productTemplate

Displays detailed information about a single product.

ratingTemplate

Displays a rating for an item.

