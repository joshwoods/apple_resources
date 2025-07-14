

- TVML
-  ratingTemplate 

# ratingTemplate

Displays a rating for an item.

## Overview

Use the `ratingTemplate` element to display a rating for an item. The following figure shows the basic layout for a `ratingTemplate` page. The theme for the rating template defaults to the system preference.

### Main Elements

The following listing shows the main elements of the `ratingTemplate` element in TVML format.

```

        …

```

#### Element Descriptions

ratingBadge  
The rating for the item.

title  
The title for the rated item.

### Example

The following listing shows the TVML for a `ratingTemplate` example. The example displays a title and a set of rating badge images, such as stars. The filled rating badge images indicate the current rating for that title. The value attribute indicates that the example title has an 80 percent favorable rating, or 4 of 5 stars.

```

        WWDC Roadtrip

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

searchTemplate

Searches for a media item based on user input.

