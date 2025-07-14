

- TVML
-  searchTemplate 

# searchTemplate

Searches for a media item based on user input.

## Overview

Use the `searchTemplate` element to display a text field that takes user input in order to search for a specific item; for example, looking for a specific movie to download. Developers can also display preselected results in a `shelf`, `list`, or `collectionList` element under the search field. The following figure shows the basic layout for a `searchTemplate` page. The theme for the search template defaults to the system preference.

### Main Elements

The following listing shows the main elements of the `searchTemplate` element in TVML format.

```

            …

                …

```

Note

The `shelf` element can be replaced with a `collectionList` or `list` element to change the look of the search results.

#### Element Descriptions

collectionList  
Element containing a group of options (such as most popular movies) or search results.

img  
A figure representing a search result.

list  
Element containing a list of options (such as most popular movies) or search results.

lockup  
A group of elements describing a search result or prepopulated results.

searchField  
A text field where the user is able to enter search terms. JavaScript is used to read the information entered.

section  
Elements that are grouped together so that they can be treated as one element for layout purposes.

shelf  
Element containing a row of options (such as most popular movies) or search results.

title  
The title for a search result.

### Example

The following listing shows the TVML for a `searchTemplate` example. The example displays a search field and keyboard along the top of the screen. A shelf is prepopulated with popular movies. Modify your main JavaScript file to accept the user input from the search field. For more information on available JavaScript functions, see TVMLKit JS.

```

                Popular

                    Movie 1

                    Movie 2

                    Movie 3

```

The following listing shows the output for the above example:

## Topics

### Valid TVML Attributes

binding

Associates information in a data item with an element.

itemID

Mark elements for reuse during DOM updates.

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

paradeTemplate

Displays a groups of items along one side of a page and scrolling images on the other side.

productBundleTemplate

Displays information for a group of related media items.

productTemplate

Displays detailed information about a single product.

ratingTemplate

Displays a rating for an item.

