

- TVML
-  catalogTemplate 

# catalogTemplate

Displays groups of items along one side of a page and images of a group’s contents on the other side.

## Overview

Use the `catalogTemplate` element to display information about groups of like products; for example, a movie catalog that provides categories for dramas, comedies, and all movies. Each group of products is contained in its own section and displayed along the left side of the screen. Images depicting the products contained within a selected group are displayed in the related content area on the right side of the screen. The following figure shows the basic layout for a `catalogTemplate` page. The theme for the catalog template defaults to the system preference.

### Main Elements

The following listing shows the main elements of the `catalogTemplate` element in TVML format.

```

      …

            …

            …

            …

```

#### Element Descriptions

banner  
Information describing what the catalog contains, such as movies.

header  
Information describing what one section of the page contains.

list  
Element containing all content in the template page, except banner information.

listItemLockup  
Element containing all information that relates to one list item on the left side of the page, including the item title and label, as well as related content.

section  
An area of the page containing related elements that are grouped together as one element for layout purposes.

### Example

The following listing shows the TVML for a `catalogTemplate` example. The example displays a title along the top of the screen. Two items representing movie categories, All Movies and Comedies, are listed along the left side of the screen. Movie posters are presented on the right in a grid format according to which movie category the user selects.

```

         Movies

               All Movies
               6

                           Movie 1

                           Movie 2

                           Movie 3

                           Movie 4

                           Movie 5

                           Movie 6

               Comedies
               4

                           Movie 2

                           Movie 1

                           Movie 4

                           Movie 3

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

searchTemplate

Searches for a media item based on user input.

