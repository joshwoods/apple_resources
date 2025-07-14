

- AppKit
-  NSStatusBar 

Class

# NSStatusBar

An object that manages a collection of status items displayed within the system-wide menu bar.

macOS

``` source
class NSStatusBar
```

## Overview

A status item (an instance of NSStatusItem) can be displayed with text or an icon, can provide a menu and a target-action message when clicked, or can be a fully customized view that you create. Use status items sparingly and only if the alternatives (such as a Dock menu, preference pane, or status window) are not suitable. Because there is limited space in which to display status items, status items are not guaranteed to be available at all times. For this reason, do not rely on them being available and always provide a user preference for hiding your application’s status items to free up space in the menu bar.

## Topics

### Getting the System-Wide Instance

class var system: NSStatusBar

Returns the system-wide status bar located in the menu bar.

### Managing Status items

func statusItem(withLength: CGFloat) -> NSStatusItem

Returns a newly created status item that has been allotted a specified space within the status bar.

func removeStatusItem(NSStatusItem)

Removes the specified status item from the receiver.

### Getting Status-Bar Attributes

var isVertical: Bool

A Boolean value indicating whether the status bar has a vertical orientation.

var thickness: CGFloat

The thickness of the status bar, in pixels.

### Constants

Status Bar Item Length

Constants used by the statusItem(withLength:) method.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Menu Bar Items

class NSStatusItem

An individual element displayed in the system menu bar.

class NSStatusBarButton

The appearance and behavior of an item in the systemwide menu bar.

