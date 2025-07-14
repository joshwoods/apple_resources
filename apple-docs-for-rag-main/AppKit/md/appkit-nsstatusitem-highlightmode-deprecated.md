

- AppKit
- NSStatusItem
-  highlightMode Deprecated

Instance Property

# highlightMode

A Boolean that indicates whether the status item is highlighted when it is clicked.

macOS 10.0–10.14Deprecated

``` source
var highlightMode: Bool { get set }
```

Deprecated

Use the button property.

## Discussion

When the value of this property is true, the status item is highlighted when it is clicked. The default value of this property is false.

## See Also

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

var toolTip: String?

The tool tip string that is displayed when the cursor pauses over the status item.

Deprecated

var view: NSView?

The custom view that is displayed at the status item’s position in the status bar.

Deprecated

func drawStatusBarBackground(in: NSRect, withHighlight: Bool)

Draws the menu background pattern for a custom status-bar item in regular or highlight pattern.

Deprecated

