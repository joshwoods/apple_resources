

- TVML
-  listTemplate 

# listTemplate

Displays a list of items along one side of a page and the corresponding image on the other side.

## Overview

Use the `listTemplate` element to display a list of items; for example, a list of the user’s favorite movies. Whereas you use the catalog template to display categories of a product (action movies, comedies, favorite movies), you use the list template to display actual contents of one category, such as a list of the user’s favorite movies. The items are listed on the right side of the screen with like items grouped together in a section. A title providing a brief description of the items is contained in a header area directly above the listed items. When an item is selected, information about the item is displayed on the left side of the screen. The following figure shows the basic layout for a `listTemplate` page. The theme for the list template defaults to the system preference.

### Main Elements

The following listing shows the main elements of the `listTemplate` in TVML format.

```

      …

         …

            …

               …

```

#### Element Descriptions

banner  
Element containing background information and the page title.

header  
Information describing what a section contains.

list  
Element containing all content for the `listTemplate` page.

listItemLockup  
Element containing all information that pertains to one list item, such as an item title and image, as well as related content.

relatedContent  
Information that is displayed on the left side of the screen when an item in the list is highlighted.

section  
An area of the page that groups related elements together as one element, for layout purposes. In this case, the section contains list items.

### Example

The following listing shows the TVML for a `listTemplate` example. An image and a description that relate to the highlighted item are displayed on the left side of the screen.

```

         Johnny Appleseed's Movie Collection

            Favorite Movies

               Movie 1

                     Movie 1
                     A brief description for the first movie should go here.

               Movie 2

                     Movie 2
                     A brief description for the second movie should go here.

               Movie 3

                     Movie 3
                     A brief description for the third movie should go here.

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

searchTemplate

Searches for a media item based on user input.

