

- UIKit
-  NSUIViewToolbarItem 

Class

# NSUIViewToolbarItem

An item in a window’s toolbar that hosts a custom UIKit view.

Mac Catalyst 16.0+

``` source
@MainActor
class NSUIViewToolbarItem
```

## Mentioned in 

Building a desktop-class iPad app

## Overview

The NSUIViewToolbarItem class lets you display a UIView in an NSToolbar. Use this class if you have a custom UIKit view you want to appear as a control in a toolbar when you build your app with Mac Catalyst.

For UIKit controls that support behavioral styles, set preferredBehavioralStyle to UIBehavioralStyle.mac if you want them to appear in the toolbar with the appearance and behavior of AppKit controls.

## Topics

### Creating a toolbar item

init(itemIdentifier: NSToolbarItem.Identifier, uiView: UIView)

Creates a toolbar item with the identifier and underlying UIKit view you specify.

### Managing the view

var uiView: UIView

The UIKit view to host in an AppKit toolbar.

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
- NSObjectProtocol
- UIPopoverPresentationControllerSourceItem

## See Also

### Items

@MainActor class NSToolbarItem

A single item that appears in a window’s toolbar.

@MainActor class NSToolbarItemGroup

A group of subitems in a toolbar item.

enum ControlRepresentation

enum SelectionMode

A value that indicates how a grouped toolbar item selects its subitems.

@MainActor class NSMenuToolbarItem

A control that presents a menu in a window’s toolbar.

@MainActor class NSSearchToolbarItem

A toolbar item that contains a search field optimized for performing text-based searches.

@MainActor class NSTrackingSeparatorToolbarItem

A toolbar separator that aligns with the vertical split view in the same window.

