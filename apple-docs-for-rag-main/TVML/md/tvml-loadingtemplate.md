

- TVML
-  loadingTemplate 

# loadingTemplate

Displays a spinner and description on the screen.

## Overview

Use the `loadingTemplate` element to display a spinner and description of why the spinner is being displayed; for example, an interim page showing that the requested page is being loaded. A spinner is automatically presented when the page is displayed, and you can add text to tell your users what is happening. The following figure shows the basic layout for a `layoutTemplate` page. The theme for the loading template defaults to the system preference.

Note

When a user performs an action to bring up a new page and the new page is not immediately ready, a `loadingTemplate` page should be presented. After the new page is ready, replace the `loadingTemplate` with the new page onto the navigation stack.

### Main Elements

The following listing shows main elements of the `loadingTemplate` in TVML format.

```

         Title

```

#### Element Descriptions

activityIndicator  
Image of a spinning wheel icon.

title  
The text telling the user why there is a delay.

### Example

The following listing shows the TVML for a loadingTemplate example.

```

         Loading requested page

```

The following figure shows the output of the above example:

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

