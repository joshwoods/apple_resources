

- AppKit
-  NSWindowTab 

Class

# NSWindowTab

A tab associated with a window that is part of a tabbing group.

macOS 10.13+

``` source
class NSWindowTab
```

## Overview

NSWindowTab describes the way a window displays as part of a tabbed window group. The properties of NSWindowTab are configurable at any time, but only take effect when the associated NSWindow displays in a tab.

AppKit automatically creates an instance of NSWindowTab for each NSWindow. You can access a window’s tab object using the tab property.

## Topics

### Customizing the Title

var title: String!

The title for the window tab.

var attributedTitle: NSAttributedString?

The title for the window tab, specified as an attributed string.

### Customizing the Tooltip

var toolTip: String!

The tooltip for this window tab.

### Adding an Accessory View

var accessoryView: NSView?

An optional accessory view for the tab.

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

var tabbingIdentifier: NSWindow.TabbingIdentifier

A value that allows a group of related windows.

### Windows

class NSWindow

A window that an app displays on the screen.

class NSPanel

A special kind of window that typically performs a function that is auxiliary to the main window.

protocol NSWindowDelegate

A set of optional methods that a window’s delegate can implement to respond to events, such as window resizing, moving, exposing, and minimizing.

class NSWindowTabGroup

A group of windows that display together as a single tabbed window.

