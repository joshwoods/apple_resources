

- AppKit
- NSRulerView
-  markers 

Instance Property

# markers

The receiver’s ruler markers to `markers`, removing any existing ruler markers and not consulting with the client view about the new markers.

macOS

``` source
@MainActor
var markers: [NSRulerMarker]? { get set }
```

## Discussion

`markers` can be `nil` or empty to remove all ruler markers. Raises an `NSInternalInconsistencyException` if `markers` is not `nil` and the receiver has no client view.

## See Also

### Related Documentation

var markerLocation: CGFloat

The location of the receiver in the coordinate system of the ruler view’s client view.

### Adding and removing markers

func addMarker(NSRulerMarker)

Adds `aMarker` to the receiver, without consulting the client view for approval.

func removeMarker(NSRulerMarker)

Removes `aMarker` from the receiver, without consulting the client view for approval.

func trackMarker(NSRulerMarker, withMouseEvent: NSEvent) -> Bool

Tracks the mouse to add `aMarker` based on the initial mouse-down or mouse-dragged event `theEvent`.

