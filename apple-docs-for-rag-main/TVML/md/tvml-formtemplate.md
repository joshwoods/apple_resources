

- TVML
-  formTemplate 

# formTemplate

Provides the ability to gather information from the user.

## Overview

Use the `formTemplate` element to gather information from the user; for example, requiring a password to access your app. The banner area can contain an image and a description of your product. The user enters text in the text field directly below the banner using the automatically generated keyboard. Use the footer area to contain any user interaction buttons. The following figure shows the basic layout for a `formTemplate` page. The theme for the form template defaults to the system preference.

### Form Template

The following listing shows the main elements of the `formTemplate` element in TVML format.

```

        …

        …

    …
    …

```

#### Element Descriptions

background  
Only accepts `img` and `heroImg` elements in the background.

banner  
Information displayed along the top of the screen that is typically used to provide instructions to the user.

description  
The text used to describe what the user needs to enter.

footer  
Information displayed along the bottom of the screen, such as a Submit button for the user to commit the information entered in `textField`.

img  
An image of the product.

textField  
User input field.

### Example

The following listing shows the TVML for a `formTemplate` example. The interactive keyboard is automatically created. The footer area contains a button that can submit the user input. Modify your main JavaScript file to accept the user input from the button. For more information on available JavaScript functions, see TVMLKit JS.

```

            Enter email for access

        tclark@example.com

                Submit

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

