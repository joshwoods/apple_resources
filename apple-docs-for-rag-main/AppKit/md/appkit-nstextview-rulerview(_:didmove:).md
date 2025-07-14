

- AppKit
- NSTextView
-  rulerView(\_:didMove:) 

Instance Method

# rulerView(\_:didMove:)

Modifies the paragraph style of the paragraphs containing the selection to record the new location of the marker.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    didMove marker: NSRulerMarker
)
```

## Parameters 

`ruler`  

The ruler view sending the message.

`marker`  

The marker that was moved.

## Discussion

This method records the change by invoking didChangeText() after moving the marker.

`NSTextView` checks for permission to make the change in its rulerView(_:shouldMove:) method, which invokes shouldChangeText(in:replacementString:) to send out the proper request and notifications, and only invokes this method if permission is granted.

## See Also

### Related Documentation

var representedObject: (any NSCopying)?

The object the receiver represents.

### Supporting the ruler view

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

func rulerView(NSRulerView, handleMouseDownWith: NSEvent)

Adds a left tab marker to the ruler at the location clicked.

