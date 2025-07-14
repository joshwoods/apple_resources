

- AppKit
- NSTextView
-  rulerView(\_:handleMouseDownWith:) 

Instance Method

# rulerView(\_:handleMouseDownWith:)

Adds a left tab marker to the ruler at the location clicked.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    handleMouseDownWith event: NSEvent
)
```

## Parameters 

`ruler`  

The ruler view sending the message.

`event`  

The mouse down event.

## Discussion

A subclass can override this method to provide other behavior, such as creating guidelines. This method is invoked once with `theEvent` when the user first clicks the ruler area of `aRulerView`, as described in the NSRulerView class specification.

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

func rulerView(NSRulerView, shouldAdd: NSRulerMarker) -> Bool

Returns whether a new marker can be added.

func rulerView(NSRulerView, willAdd: NSRulerMarker, atLocation: CGFloat) -> CGFloat

Returns a potentially modified location to which the marker should be added.

