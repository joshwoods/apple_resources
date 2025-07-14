

- TVML
-  menuBarTemplate 

# menuBarTemplate

Creates a page with items along the top and related information below.

## Overview

Use the `menuBarTemplate` to display a list of selectable items across the top of the screen. Users can move between menu bar items to change the information displayed below the menu bar. The following figure shows the basic layout for a `menuBarTemplate` page. The theme for the menu bar template defaults to the system preference.

Note

You can display up to seven items in the menu bar.

### Main Elements

The following listing shows the main elements of the `menuBarTemplate` element in TVML format.

```

                …

```

#### Element Descriptions

menuBar  
Menu items associated with the menu bar.

menuItem  
Information about a single menu item.

title  
The text that describes the menu item.

### Example

The following listing shows the TVML for a `menuBarTemplate` example. The example shows the menu bar along the top of the screen. Expand the controlling JavaScript file in order to show content for each item in the menu bar. For more information, see TVMLKit JS.

```

                Top Movies

                Genres

                Search

                Edit

                Add Settings

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

