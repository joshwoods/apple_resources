

- TVML
-  oneupTemplate 

# oneupTemplate

Creates a page that allows users to navigate between full-screen images.

## Overview

Use the `oneupTemplate` element to display a single, full-screen image. Users can navigate left or right on the remote to select another image. Activating an up action on the remote will shrink the image and allow a description to be displayed. The following figure shows the basic layout for a `oneupTemplate` page. The default theme for a oneup template is `dark`.

### Main Elements

The following listing shows the main elements of the `oneupTemplate` element in TVML format.

```

            …

                …

            …

```

#### Element Descriptions

img  
The image to be displayed on screen.

lockup  
A single image and related text.

row  
Subtitle information relating to the selected image.

section  
Multiple `lockup` elements, each of which contains an item to be displayed.

title  
The title to be displayed when a user selects an image.

### Example

The following listing shows the TVML for a `oneupTemplate` example. The example shows a full screen image, with information about the image displayed along the bottom of the screen when the user zooms into the image.

```

                WWDC Roadtrip

                    San Francisco
                    June 8, 2015

                Beach time

                    Santa Cruz
                    May 1, 2015

                Spaced out

                    Space station
                    July 15, 2015

```

The following figure shows the output for the above example:

## Topics

### Valid TVML Styles

tv-transition

Specifies how an element transitions on and off the screen.

### Valid TVML Attributes

binding

Associates information in a data item with an element.

layoutDirection

Specifies the direction in which text is displayed.

mode

Specifies how an image is displayed.

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

