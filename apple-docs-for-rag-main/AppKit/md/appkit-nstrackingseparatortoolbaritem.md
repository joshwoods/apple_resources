

- AppKit
-  NSTrackingSeparatorToolbarItem 

Class

# NSTrackingSeparatorToolbarItem

A toolbar separator that aligns with the vertical split view in the same window.

macOS 11.0+

``` source
@MainActor
class NSTrackingSeparatorToolbarItem
```

## Overview

Use a `NSTrackingSeparatorToolbarItem` to divide an NSToolbar into sections that visually align with the views on either side of the divider of the splitView. This keeps NSToolbarItems above the content that’s the target for the item’s target.

The `splitView` must be in the same window as the toolbar containing this item before showing the toolbar.

## Topics

### Creating a tracking separator

convenience init(identifier: NSToolbarItem.Identifier, splitView: NSSplitView, dividerIndex: Int)

Creates a new tracking separator toolbar item and configures it to align with the divider of the split view.

### configuring a tracking separator

var dividerIndex: Int

The index of the split view divider to align with the tracking separator.

var splitView: NSSplitView

The vertical split view to align with the toolbar separator.

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
- Sendable

## See Also

### Items

class NSToolbarItem

A single item that appears in a window’s toolbar.

class NSToolbarItemGroup

A group of subitems in a toolbar item.

enum ControlRepresentation

enum SelectionMode

A value that indicates how a grouped toolbar item selects its subitems.

class NSMenuToolbarItem

A control that presents a menu in a window’s toolbar.

class NSSearchToolbarItem

A toolbar item that contains a search field optimized for performing text-based searches.

