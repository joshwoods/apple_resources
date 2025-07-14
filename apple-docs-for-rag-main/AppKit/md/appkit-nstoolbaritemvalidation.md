

- AppKit
-  NSToolbarItemValidation 

Protocol

# NSToolbarItemValidation

Validation of a toolbar item.

macOS

``` source
protocol NSToolbarItemValidation : NSObjectProtocol
```

## Overview

A toolbar item with a valid target and action is enabled by default. To allow a toolbar item to be disabled in certain situations, a toolbar item’s target can implement the validateToolbarItem(_:) method.

Note

The NSToolbarItem validate() method is called only if the item’s target has a valid action defined on its target and if the item isn’t a custom view item. If you want to validate a custom view item, then you have to subclass NSToolbarItem and override validate().

## Topics

### Enabling and disabling toolbar items

func validateToolbarItem(NSToolbarItem) -> Bool

If this method is implemented and returns false, NSToolbar will disable `theItem`; returning true causes `theItem` to be enabled.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### View

Integrating a Toolbar and Touch Bar into Your App

Provide users quick access to your app’s features from a toolbar and corresponding Touch Bar.

class NSToolbar

An object that manages the space above your app’s custom content and either below or integrated with the window’s title bar.

