

- AppKit
- NSTextView
-  rulerView(\_:shouldAdd:) 

Instance Method

# rulerView(\_:shouldAdd:)

Returns whether a new marker can be added.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    shouldAdd marker: NSRulerMarker
) -> Bool
```

## Parameters 

`ruler`  

The ruler view sending the message.

`marker`  

The marker to be added.

## Return Value

true if `aMarker` can be added, false otherwise.

## Discussion

The receiver checks for permission to make the change by invoking shouldChangeText(in:replacementString:) and returning the return value of that message. If the change is allowed, the receiver is then sent a rulerView(_:didAdd:) message.

## See Also

### Supporting the ruler view

func rulerView(NSRulerView, didMove: NSRulerMarker)

Modifies the paragraph style of the paragraphs containing the selection to record the new location of the marker.

func rulerView(NSRulerView, willMove: NSRulerMarker, toLocation: CGFloat) -> CGFloat

Returns a potentially modified location to which the marker should be moved.

func rulerView(NSRulerView, shouldMove: NSRulerMarker) -> Bool

Returns whether the marker should be moved.

func rulerView(NSRulerView, didRemove: NSRulerMarker)

Modifies the paragraph style of the paragraphs containing the selection—if possible—by removing the specified marker.

func rulerView(NSRulerView, shouldRemove: NSRulerMarker) -> Bool

Returns whether the marker should be removed.

func rulerView(NSRulerView, didAdd: NSRulerMarker)

Modifies the paragraph style of the paragraphs containing the selection to accommodate a new marker.

func rulerView(NSRulerView, willAdd: NSRulerMarker, atLocation: CGFloat) -> CGFloat

Returns a potentially modified location to which the marker should be added.

func rulerView(NSRulerView, handleMouseDownWith: NSEvent)

Adds a left tab marker to the ruler at the location clicked.

