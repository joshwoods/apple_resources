

- AppKit
- NSTextView
-  rulerView(\_:shouldRemove:) 

Instance Method

# rulerView(\_:shouldRemove:)

Returns whether the marker should be removed.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    shouldRemove marker: NSRulerMarker
) -> Bool
```

## Parameters 

`ruler`  

The ruler view sending the message.

`marker`  

The marker to be removed.

## Return Value

true if `aMarker` can be removed, false otherwise.

## Discussion

Only markers that represent tab stops can be removed. This method returns true if `aMarker` represents an NSTextTab object, false otherwise. Because this method can be invoked repeatedly as the user drags a ruler marker, it returns that value immediately. If the change is allowed and the user actually removes the marker, the receiver is also sent a rulerView(_:didRemove:) message.

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

func rulerView(NSRulerView, didAdd: NSRulerMarker)

Modifies the paragraph style of the paragraphs containing the selection to accommodate a new marker.

func rulerView(NSRulerView, shouldAdd: NSRulerMarker) -> Bool

Returns whether a new marker can be added.

func rulerView(NSRulerView, willAdd: NSRulerMarker, atLocation: CGFloat) -> CGFloat

Returns a potentially modified location to which the marker should be added.

func rulerView(NSRulerView, handleMouseDownWith: NSEvent)

Adds a left tab marker to the ruler at the location clicked.

