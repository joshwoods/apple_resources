

- TVML
-  descriptiveAlertTemplate 

# descriptiveAlertTemplate

Displays large amounts of important information to the user.

## Overview

Use the `descriptiveAlertTemplate` element to display a significant amount of important information, such as a Terms of Service page. A title is displayed at the top of the screen with a large text area directly below it. An area containing buttons is located along the bottom of the screen. The following figure shows the basic layout for a `descriptiveAlertTemplate` page. The theme for the descriptive alert template defaults to the system preference.

### Main Elements

The following listing shows the main elements of the `descriptiveAlertTemplate` in TVML format.

```

      …

   Title

   Description

         …

```

#### Element Descriptions

background  
Background elements, such as audio.

button  
A button for the alert. A button typically lets the user dismiss the alert or bring up a new template page.

description  
The main text for the alert.

img  
An image associated with the alert box.

row  
A row of buttons.

title  
The title for the descriptive alert page.

### Example

The following listing shows the TVML for a `descriptiveAlertTemplate` example.

```

      Terms of Service
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum

            Accept

            Decline

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

