

- AppKit
-  NSMenuToolbarItem 

Class

# NSMenuToolbarItem

A control that presents a menu in a window’s toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
class NSMenuToolbarItem
```

## Overview

If you set an action on an NSMenuToolbarItem control item, the user invokes the action when clicking on the item through pressing and holding to display the menu. If you set an action on the item and showsIndicator to true, the system displays the indicator as a separate segment so the user can invoke the menu with a click on that segment.

If you don’t set an action on the NSMenuToolbarItem, a simple click invokes the menu, and the indicator is purely decorative.

## Topics

### Configuring a menu toolbar item

var showsIndicator: Bool

A Boolean value that determines whether the toolbar item displays an indicator of additional functionality.

var menu: NSMenu

The menu presented from the toolbar item.

var itemMenu: UIMenu

## Relationships

### Inherits From

- NSToolbarItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMenuItemValidation
- NSObjectProtocol
- NSValidatedUserInterfaceItem

## See Also

### Items

class NSToolbarItem

A single item that appears in a window’s toolbar.

class NSToolbarItemGroup

A group of subitems in a toolbar item.

enum ControlRepresentation

enum SelectionMode

A value that indicates how a grouped toolbar item selects its subitems.

class NSSearchToolbarItem

A toolbar item that contains a search field optimized for performing text-based searches.

class NSTrackingSeparatorToolbarItem

A toolbar separator that aligns with the vertical split view in the same window.

