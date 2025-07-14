

- TVML
-  mainTemplate 

# mainTemplate

Displays user options for a media item.

## Overview

Use the `mainTemplate` element to display options to the user; for example, the main page for a movie with options to play the movie, see extra content, and jump to specific scenes. The background area contains an image relating to the product, and the options are contained in a menu bar along the bottom of the screen. The following figure shows the basic layout for a `mainTemplate` page. The default theme for a main template is `dark`.

### Main Elements

The following listing shows the elements of the mainTemplate element in TVML format.

```

    …

            …
            …

```

#### Element Descriptions

background  
The background elements used on the page, such as `audio`.

menuBar  
A list of displayed menu items.

menuItem  
Information for an individual menu item.

section  
An area containing a group of menu items.

### Example

The following listing shows the TVML for a `mainTemplate` example. The example displays a full-screen image as the background. A menu bar contains three navigable options.

```

                    PLAY

                    SCENES

                    EXTRAS

```

The following figure shows the output for the above example:

## Topics

### Valid TVML Attributes

binding

Associates information in a data item with an element.

layoutDirection

Specifies the direction in which text is displayed.

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

searchTemplate

Searches for a media item based on user input.

