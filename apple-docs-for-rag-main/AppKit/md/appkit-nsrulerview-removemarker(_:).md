

- AppKit
- NSRulerView
-  removeMarker(\_:) 

Instance Method

# removeMarker(\_:)

Removes `aMarker` from the receiver, without consulting the client view for approval.

macOS

``` source
@MainActor
func removeMarker(_ marker: NSRulerMarker)
```

## See Also

### Adding and removing markers

var markers: [NSRulerMarker]?

The receiver’s ruler markers to `markers`, removing any existing ruler markers and not consulting with the client view about the new markers.

func addMarker(NSRulerMarker)

Adds `aMarker` to the receiver, without consulting the client view for approval.

func trackMarker(NSRulerMarker, withMouseEvent: NSEvent) -> Bool

Tracks the mouse to add `aMarker` based on the initial mouse-down or mouse-dragged event `theEvent`.

