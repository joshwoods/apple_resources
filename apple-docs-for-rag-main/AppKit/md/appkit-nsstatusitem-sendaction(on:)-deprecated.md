

- AppKit
- NSStatusItem
-  sendAction(on:) Deprecated

Instance Method

# sendAction(on:)

Sets the conditions on which the status item sends action messages to its target.

macOS 10.0–10.14Deprecated

``` source
func sendAction(on mask: NSEvent.EventTypeMask) -> Int
```

Deprecated

Use the button property.

## Parameters 

`mask`  

Takes one or more of the following bit masks described in `Getting Unicode Values` section of the `NSEvent` class reference: `NSLeftMouseUpMask`, `NSLeftMouseDownMask`, `NSLeftMouseDraggedMask`, and `NSPeriodicMask`. Bitwise-OR multiple bit masks.

## Return Value

A bit mask containing the previous settings. This bit mask uses the same values as specified in the `mask` parameter.

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

