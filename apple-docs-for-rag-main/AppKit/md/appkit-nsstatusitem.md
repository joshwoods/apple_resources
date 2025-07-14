

- AppKit
-  NSStatusItem 

Class

# NSStatusItem

An individual element displayed in the system menu bar.

macOS

``` source
class NSStatusItem
```

## Overview

The NSStatusBar method statusItem(withLength:) creates instances of this class and automatically adds them to the menu bar. Use the button property to customize the appearance and behavior of the status item.

## Topics

### Getting the Item’s Status Bar

var statusBar: NSStatusBar?

The status bar that displays the status item.

### Managing the Status Item’s Behavior

var behavior: NSStatusItem.Behavior

The set of allowed behaviors for the status item.

struct Behavior

A set of optional status item behaviors.

var button: NSStatusBarButton?

The button displayed in the status bar.

var menu: NSMenu?

The pull-down menu displayed when the user clicks the status item.

### Configuring the Status Item’s Appearance

var isVisible: Bool

A Boolean value indicating if the menu bar currently displays the status item.

var length: CGFloat

The amount of space in the status bar that should be allocated to the status item.

class let squareLength: CGFloat

A status item length that is equal to the status bar’s thickness.

class let variableLength: CGFloat

A status item length that dynamically adjusts to the width of its contents.

### Setting the Autosave Name

var autosaveName: NSStatusItem.AutosaveName!

A unique name for saving and restoring information about a status item.

typealias AutosaveName

### Deprecated

var isEnabled: Bool

A Boolean that indicates whether the status item is enabled to respond to clicks.

Deprecated

var target: AnyObject?

The target object to which the status item’s action message is sent when the status item is clicked.

Deprecated

var action: Selector?

The selector that is sent to the status item’s target when the status item is clicked.

Deprecated

var doubleAction: Selector?

The selector that is sent to the status item’s target when the status item is double-clicked.

Deprecated

func sendAction(on: NSEvent.EventTypeMask) -> Int

Sets the conditions on which the status item sends action messages to its target.

Deprecated

func popUpMenu(NSMenu)

Displays a menu under a custom status bar item.

Deprecated

var title: String?

The string that is displayed at the status item’s position in the status bar.

Deprecated

var attributedTitle: NSAttributedString?

The attributed string that is displayed at the status item’s position in the status bar.

Deprecated

var image: NSImage?

The image that is displayed at the status item’s position in the status bar.

Deprecated

var alternateImage: NSImage?

The alternate image to be displayed when a status bar item is highlighted.

Deprecated

var highlightMode: Bool

A Boolean that indicates whether the status item is highlighted when it is clicked.

Deprecated

var toolTip: String?

The tool tip string that is displayed when the cursor pauses over the status item.

Deprecated

var view: NSView?

The custom view that is displayed at the status item’s position in the status bar.

Deprecated

func drawStatusBarBackground(in: NSRect, withHighlight: Bool)

Draws the menu background pattern for a custom status-bar item in regular or highlight pattern.

Deprecated

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

class NSStatusBar

An object that manages a collection of status items displayed within the system-wide menu bar.

class NSStatusBarButton

The appearance and behavior of an item in the systemwide menu bar.

