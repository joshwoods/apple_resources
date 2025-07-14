

- TVML
-  divTemplate 

# divTemplate

Provides the ability to create pages that don’t conform to a layout defined by another template.

## Overview

There is no built-in layout for contained elements. The `divTemplate` element creates a view where the elements it contains are arranged using the `tv-align` and `tv-position` styles. Containing elements are centered by default. The following figure shows the positions inside of the `divTemplate` element. The `divTemplate` element should only be used when you can’t use another template to achieve the look you want. The theme for the div template defaults to the system preference.

Elements contained in the same position are arranged from the top of the cell to the bottom, in the same order in which they are specified in the `divTemplate` element. You can specify a `` that displays a background image inside of the `divTemplate`. The background image is top-aligned and is fitted to the size of the `divTemplate` while keeping the image’s original aspect ratio. Text wrapping inside of the `divTemplate` only occurs in the `header`, `center`, and `footer` positions.

## Topics

### Valid TVML Styles

tv-align

Aligns an element horizontally inside its parent.

tv-position

Sets the position of an element inside of its parent element.

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

