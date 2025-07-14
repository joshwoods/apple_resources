

- AppKit
- NSTextView
-  rulerView(\_:willMove:toLocation:) 

Instance Method

# rulerView(\_:willMove:toLocation:)

Returns a potentially modified location to which the marker should be moved.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    willMove marker: NSRulerMarker,
    toLocation location: CGFloat
) -> CGFloat
```

## Parameters 

`ruler`  

The ruler view sending the message.

`marker`  

The marker to be moved.

`location`  

The new location for the marker, in the ruler view’s coordinates.

## Return Value

The modified location to which the marker should be moved.

## Discussion

This method ensures that the proposed `location` of `aMarker` lies within the appropriate bounds for the receiver’s text container. Appropriate bounds are those of the text container minus its line fragment padding.

Typically, the ruler view’s width matches that of its text view.

## See Also

### Supporting the ruler view

func rulerView(NSRulerView, didMove: NSRulerMarker)

Modifies the paragraph style of the paragraphs containing the selection to record the new location of the marker.

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

func rulerView(NSRulerView, handleMouseDownWith: NSEvent)

Adds a left tab marker to the ruler at the location clicked.

