

- Safari Services
-  SFSafariToolbarItem 

Class

# SFSafariToolbarItem

A proxy for a Safari app extension toolbar item in a Safari window.

macOS 10.12+

``` source
class SFSafariToolbarItem
```

## Overview

Your app extension only uses this object when it wants to explicitly set the toolbar item state. Typically, other state changes occur automatically. Safari calls validateToolbarItem(in:validationHandler:) on your app extension handler when changes, such as navigation to a webpage, could affect the state of the toolbar item.

## Topics

### Controlling Toolbar Items

func setEnabled(Bool, withBadgeText: String?)

Sets the enabled state and the badge text for the toolbar item.

Deprecated

func setBadgeText(String?)

Sets the badge text for the toolbar item.

func setEnabled(Bool)

Sets whether the toolbar item is enabled.

func setImage(NSImage?)

Sets the image displayed in the toolbar button.

func setLabel(String?)

### Instance Methods

func showPopover()

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Contextual menu and toolbar items

Using contextual menu and toolbar item keys

Learn about adding contextual menu items and toolbar items to a Safari app extension with information property list keys.

Adjusting settings for a toolbar item

Customize a toolbar item for your Safari app extension.

Adjusting settings for contextual menu items

Customize contextual menu items for your Safari app extension.

class SFSafariExtensionViewController

The view controller for a popover associated with your app extension.

