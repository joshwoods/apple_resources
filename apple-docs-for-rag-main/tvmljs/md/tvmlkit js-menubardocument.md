

- TVMLKit JS
-  MenuBarDocument 

Class

# MenuBarDocument

An object used for setting and retrieving documents associated with a menu item.

tvOS 9.0+

``` source
interface MenuBarDocument
```

## Overview

Use the `getFeature` function with the feature name `MenuBarDocument` to retrieve an instance of this class from the `menuBar` element; for example, `getFeature('MenuBarDocument')`.

## Topics

### Setting and Retrieving Menu Item Documents

getDocument

Retrieves the document associated with the specified menu item.

getSelectedItem

Retrieves the menu item in the menu bar that is currently in focus.

setDocument

Associates a document with a menu item.

setSelectedItem

Sets the focus in a menu bar to the specified menu item.

## See Also

### Element Access

Keyboard

An object used to retrieve user input from search fields and text fields.

