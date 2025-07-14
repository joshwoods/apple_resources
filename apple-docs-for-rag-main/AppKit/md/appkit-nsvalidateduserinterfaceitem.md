

- AppKit
-  NSValidatedUserInterfaceItem 

Protocol

# NSValidatedUserInterfaceItem

A protocol that a custom class can adopt to manage the automatic enablement of a UI control.

macOS

``` source
protocol NSValidatedUserInterfaceItem
```

## Overview

The NSValidatedUserInterfaceItem protocol works with the NSUserInterfaceValidations protocol to enable or disable a control automatically, depending on whether any responder in the responder chain can handle the control’s action method. The NSMenuItem and NSToolbarItem classes implement this protocol.

By conforming to this protocol, your control can participate in this validation mechanism. To validate a control, the application calls validateUserInterfaceItem(_:) for each item in the responder chain, starting with the first responder. If no responder returns true, the item is disabled. For example, a menu item that sends the `copy:` action message would disable itself if no responder in the responder chain can be copied.

## Topics

### Getting information about a user interface item

var action: Selector?

Returns the selector of the receiver’s action method.

**Required**

var tag: Int

Returns the receiver’s tag integer.

**Required**

## Relationships

### Conforming Types

- NSMenuItem
- NSMenuToolbarItem
- NSSearchToolbarItem
- NSSharingServicePickerToolbarItem
- NSToolbarItem
- NSToolbarItemGroup
- NSTrackingSeparatorToolbarItem

## See Also

### UI Validation

protocol NSUserInterfaceValidations

A protocol that a custom class can adopt to manage the enabled state of a UI element.

