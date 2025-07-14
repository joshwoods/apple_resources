

- TVML
-  paradeTemplate 

# paradeTemplate

Displays a groups of items along one side of a page and scrolling images on the other side.

## Overview

Use the `paradeTemplate` element to display a list of automatically scrolling, static images on the left that are associated with a selected image category on the right. For example, a user selects Action movies, and the associated images automatically start scrolling. The following figure shows the basic layout for a `paradeTemplate` page. The theme for the parade template defaults to the system preference.

### Main Elements

The following listing shows main elements of the `paradeTemplate` in TVML format.

```

         Title

            Title 1

            Title 2

```

#### Element Descriptions

header  
Title information for the list of image categories on the right side of the screen.

img  
A single image that scrolls across the left side of the screen.

imgDeck  
A group of images on the left side of the screen that scroll right-to-left.

list  
Element containing all the elements that are displayed.

listItemLockup  
Information about an individual item in the list of image categories.

relatedContent  
Element containing the image deck that is associated with a particular item in the list.

title  
The text used to provide a description for its containing element.

### Example

The following listing shows the TVML for a `paradeTemplate` example.

```

                Movie Genres

                    Action

                    Comedy

                    Horror

                    Kids

                    Drama

```

The following figure shows the output for the above example:

## Topics

### Valid TVML Attributes

autoHighlight

Specifies that the element should initially be in focus.

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

mainTemplate

Displays user options for a media item.

menuBarTemplate

Creates a page with items along the top and related information below.

oneupTemplate

Creates a page that allows users to navigate between full-screen images.

productBundleTemplate

Displays information for a group of related media items.

productTemplate

Displays detailed information about a single product.

ratingTemplate

Displays a rating for an item.

searchTemplate

Searches for a media item based on user input.

