

- AppKit
- NSRulerMarker
-  trackMouse(with:adding:) 

Instance Method

# trackMouse(with:adding:)

Handles user manipulation of the receiver in its ruler view.

macOS

``` source
func trackMouse(
    with mouseDownEvent: NSEvent,
    adding isAdding: Bool
) -> Bool
```

## Parameters 

`mouseDownEvent`  

The event that represents the user manipulation being attempted on the ruler marker.

`isAdding`  

true to indicate that the receiver is a new marker being added to its ruler view, false otherwise.

## Return Value

true if the user manipulation was allowed, false if it was not allowed.

## Discussion

NSRulerView objects invoke this method automatically to add a new marker or to move or remove an existing marker. You should never need to invoke it directly.

If the receiver is a new marker being added to its ruler view (`flag` is true), the receiver queries the ruler view’s client before adding itself to the ruler view. If the client responds to rulerView(_:shouldAdd:) and that method returns false, this method immediately returns false, and the new marker isn’t added.

If the receiver is not a new marker being added to its ruler view (`flag` is false), this method attempts to move or remove an existing marker, once again based on responses from the ruler view’s client view. If the receiver is neither movable nor removable, this method immediately returns false. Further, if the ruler view’s client responds to rulerView(_:shouldMove:) and returns false, this method returns false, indicating the receiver can’t be moved.

If the receiver is being added or moved, this method queries the client view using rulerView(_:willAdd:atLocation:) or rulerView(_:willMove:toLocation:), respectively. If the client responds to the method, the return value is used as the receiver’s location. These methods are invoked repeatedly as the receiver is dragged within the ruler view.

If the receiver is an existing marker being removed (dragged off the ruler), this method queries the client view using rulerView(_:shouldRemove:). If the client responds to this method and returns false, the marker is pinned to the ruler view’s baseline (following the cursor on the baseline if it’s movable).

When the user releases the mouse button, this method informs the client view of the marker’s new status using rulerView(_:didAdd:), rulerView(_:didMove:), or rulerView(_:didRemove:) as appropriate. The client view can use this notification to set the marker’s represented object, modify its state and redisplay (for example, adjusting text layout around a new tab stop), or take whatever other action it might need.

If `flag` is true and the user dragged the new marker away from the ruler, the marker isn’t added, no message is sent, and this method returns false.

See Ruler and Paragraph Style Programming Topics for more information on these client methods.

## See Also

### Related Documentation

var isMovable: Bool

A Boolean that indicates whether the user can move the receiver in its ruler view.

var isRemovable: Bool

A Boolean that indicates whether the user can remove the receiver from its ruler view.

### Drawing and event handling

func draw(NSRect)

Draws the receiver’s image that appears in the supplied rectangle.

var isDragging: Bool

A Boolean that indicates whether the receiver is being dragged.

