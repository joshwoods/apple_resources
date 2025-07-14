

- Safari Services
-  SFSafariExtensionViewController 

Class

# SFSafariExtensionViewController

The view controller for a popover associated with your app extension.

macOS 10.12+

``` source
@MainActor
class SFSafariExtensionViewController
```

## Mentioned in 

Adjusting settings for a toolbar item

## Overview

If your toolbar item has a popover, your popover view controller should be a subclass of this class. As with other macOS development, typically you want to add your own outlets and actions to the view controller, and provide an XIB file for its user interface.

Your view controller’s contents must use Auto Layout.

## Topics

### Instance Methods

func dismissPopover()

## Relationships

### Inherits From

- NSViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

## See Also

### Contextual menu and toolbar items

Using contextual menu and toolbar item keys

Learn about adding contextual menu items and toolbar items to a Safari app extension with information property list keys.

Adjusting settings for a toolbar item

Customize a toolbar item for your Safari app extension.

Adjusting settings for contextual menu items

Customize contextual menu items for your Safari app extension.

class SFSafariToolbarItem

A proxy for a Safari app extension toolbar item in a Safari window.

