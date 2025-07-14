

- AppKit
- NSTextView
-  rulerView(\_:shouldMove:) 

Instance Method

# rulerView(\_:shouldMove:)

Returns whether the marker should be moved.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    shouldMove marker: NSRulerMarker
) -> Bool
```

## Parameters 

`ruler`  

The ruler view sending the message.

`marker`  

The marker to be moved.

## Return Value

true if `aMarker` can be moved, false otherwise.

## Discussion

This method controls whether an existing marker `aMarker` can be moved. The receiver checks for permission to make the change by invoking shouldChangeText(in:replacementString:) and returning the return value of that message. If the change is allowed, the receiver is then sent a rulerView(_:didMove:) message.

## See Also

### Supporting the ruler view

func rulerView(NSRulerView, didMove: NSRulerMarker)

Modifies the paragraph style of the paragraphs containing the selection to record the new location of the marker.

func rulerView(NSRulerView, willMove: NSRulerMarker, toLocation: CGFloat) -> CGFloat

Returns a potentially modified location to which the marker should be moved.

func rulerView(NSRulerView, didRemove: NSRulerMarker)

Modifies the paragraph style of the paragraphs containing the selection—if possible—by removing the specified marker.

func rulerView(NSRulerView, shouldRemove: NSRulerMarker) -> Bool

Returns whether the marker should be removed.

func rulerView(NSRulerView, didAdd: NSRulerMarker)

Modifies the paragraph style of the paragraphs containing the selection to accommodate a new marker.

func rulerView(NSRulerView, shouldAdd: NSRulerMarker) -> Bool

Returns whether a new marker can be added.

func rulerView(NSRulerView, willAdd: NSRulerMarker, atLocation: CGFloat) -> CGFloat

Returns a potentially modified location to which the marker should be added.

func rulerView(NSRulerView, handleMouseDownWith: NSEvent)

Adds a left tab marker to the ruler at the location clicked.

