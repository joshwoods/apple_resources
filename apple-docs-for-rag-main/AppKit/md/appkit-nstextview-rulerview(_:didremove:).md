

- AppKit
- NSTextView
-  rulerView(\_:didRemove:) 

Instance Method

# rulerView(\_:didRemove:)

Modifies the paragraph style of the paragraphs containing the selection—if possible—by removing the specified marker.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    didRemove marker: NSRulerMarker
)
```

## Parameters 

`ruler`  

The ruler view sending the message.

`marker`  

The marker that was removed.

## Discussion

This method records the change by invoking didChangeText() after removing the marker.

`NSTextView` checks for permission to move or remove a tab stop in its rulerView(_:shouldMove:) method, which invokes shouldChangeText(in:replacementString:) to send out the proper request and notifications, and only invokes this method if permission is granted.

## See Also

### Related Documentation

var representedObject: (any NSCopying)?

The object the receiver represents.

func shouldChangeText(in: NSRange, replacementString: String?) -> Bool

Initiates a series of delegate messages (and general notifications) to determine whether modifications can be made to the characters and attributes of the receiver’s text.

### Supporting the ruler view

func rulerView(NSRulerView, didMove: NSRulerMarker)

Modifies the paragraph style of the paragraphs containing the selection to record the new location of the marker.

func rulerView(NSRulerView, willMove: NSRulerMarker, toLocation: CGFloat) -> CGFloat

Returns a potentially modified location to which the marker should be moved.

func rulerView(NSRulerView, shouldMove: NSRulerMarker) -> Bool

Returns whether the marker should be moved.

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

