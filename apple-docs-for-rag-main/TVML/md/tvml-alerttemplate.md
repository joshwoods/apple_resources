

- TVML
-  alertTemplate 

# alertTemplate

Displays important information to the user.

## Overview

Use the `alertTemplate` element to display important information, such as a message telling the user to perform an action before continuing. At a minimum, provide a description of the alert and a button so the user can take any required actions. The following figure shows the basic layout for an `alertTemplate` page. The theme for the alert template defaults to the system preference.

### Main Elements

The following listing shows the main elements of the `alertTemplate` element in TVML format:

```
```

#### Element Descriptions

background  
Background elements, such as audio.

button  
A button that typically allows the user to dismiss the alert or to bring up a new template page. The button element contains a text element that shows the name of the button.

description  
The main text for the alert.

text  
A brief description of what the button does.

title  
The title of the alert, which should briefly communicate its purpose.

### Example

The following listing shows the TVML for an `alertTemplate` example:

```
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

searchTemplate

Searches for a media item based on user input.

