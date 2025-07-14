

- TVML
-  showcaseTemplate 

# showcaseTemplate

Displays images the user can navigate between.

## Overview

Use the `showcaseTemplate` element to display a row of images with descriptions associated with each image; for example, displaying a set of screenshots to promote a movie. Users can scroll between images. When an image comes into focus, the size of the image is increased to be slightly larger than the other images. The following figure shows the basic layout for a showcaseTemplate page. The default theme for a showcase template is `dark`.

### Main Elements

The following listing shows the main elements of the `showcaseTemplate` element in TVML format.

```

    …

        …

            …

            …

```

#### Element Descriptions

background  
Background visual and audio.

banner  
Elements that describe what the page shows and provides buttons for user options.

button  
A button providing user options.

carousel  
Element containing images and text displayed in a row that the user navigates by swiping left or right on the remote.

lockup  
An element containing several elements, such as an image and a title, so that it can be treated as a single element.

row  
A group of elements displayed in a horizontal row.

section  
A group of `lockup` elements.

title  
Text that describes its containing element.

### Example

The following listing shows the TVML for a `showcaseTemplate` example.

```

            Scenes

                    Slideshow

                    Screensaver

                    Scene 1

                    Scene 2

                    Scene 3

                    Scene 4

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

