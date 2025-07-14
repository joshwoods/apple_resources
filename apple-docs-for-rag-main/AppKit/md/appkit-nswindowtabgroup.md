

- AppKit
-  NSWindowTabGroup 

Class

# NSWindowTabGroup

A group of windows that display together as a single tabbed window.

macOS 10.13+

``` source
class NSWindowTabGroup
```

## Overview

AppKit automatically creates instances of NSWindowTabGroup to reflect the tabbing state of your windows. You can access a window’s current tab group using the tabGroup property.

## Topics

### Checking the Group Identifier

var identifier: NSWindow.TabbingIdentifier

The unique identifier for a tabbed window group.

### Configuring the Tab User Interface

var isOverviewVisible: Bool

A Boolean value indicating if the tab overview is currently displayed.

var isTabBarVisible: Bool

A Boolean value indicating whether the tabbed window group currently displays a tab bar.

### Managing Tabbed Windows

var windows: [NSWindow]

A collection of the windows that are currently grouped together by this window tab group.

var selectedWindow: NSWindow?

The selected, or frontmost, window in the tab group.

func addWindow(NSWindow)

Adds a window to the tab group.

func insertWindow(NSWindow, at: Int)

Inserts a window at a specific location within the tab group.

func removeWindow(NSWindow)

Removes a window from the tab group.

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

### Related Documentation

var tabGroup: NSWindowTabGroup?

A group of windows that display together as a tab group.

### Windows

class NSWindow

A window that an app displays on the screen.

class NSPanel

A special kind of window that typically performs a function that is auxiliary to the main window.

protocol NSWindowDelegate

A set of optional methods that a window’s delegate can implement to respond to events, such as window resizing, moving, exposing, and minimizing.

class NSWindowTab

A tab associated with a window that is part of a tabbing group.

