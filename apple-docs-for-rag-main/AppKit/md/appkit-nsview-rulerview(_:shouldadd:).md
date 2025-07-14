

- AppKit
- NSView
-  rulerView(\_:shouldAdd:) 

Instance Method

# rulerView(\_:shouldAdd:)

Requests permission for `aRulerView` to add `aMarker`, an NSRulerMarker being dragged onto the ruler by the user.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    shouldAdd marker: NSRulerMarker
) -> Bool
```

## Discussion

If the client returns true the ruler view accepts the new marker and begins tracking its movement; if the client returns false the ruler view refuses the new marker.

## See Also

### Synchronizing with Ruler Views

func rulerView(NSRulerView, didAdd: NSRulerMarker)

Informs the client that `aRulerView` allowed the user to add `aMarker`.

func rulerView(NSRulerView, didMove: NSRulerMarker)

Informs the client that `aRulerView` allowed the user to move `aMarker`.

func rulerView(NSRulerView, didRemove: NSRulerMarker)

Informs the client that `aRulerView` allowed the user to remove `aMarker`.

func rulerView(NSRulerView, handleMouseDownWith: NSEvent)

Informs the client that the user has pressed the mouse button while the cursor is in the ruler area of `aRulerView`.

func rulerView(NSRulerView, locationFor: NSPoint) -> CGFloat

func rulerView(NSRulerView, pointForLocation: CGFloat) -> NSPoint

func rulerView(NSRulerView, shouldMove: NSRulerMarker) -> Bool

Requests permission for `aRulerView` to move `aMarker`.

func rulerView(NSRulerView, shouldRemove: NSRulerMarker) -> Bool

Requests permission for `aRulerView` to remove `aMarker`.

func rulerView(NSRulerView, willAdd: NSRulerMarker, atLocation: CGFloat) -> CGFloat

Informs the client that `aRulerView` will add the new NSRulerMarker, `aMarker`.

func rulerView(NSRulerView, willMove: NSRulerMarker, toLocation: CGFloat) -> CGFloat

Informs the client that `aRulerView` will move `aMarker`, an NSRulerMarker already on the ruler view.

func rulerView(NSRulerView, willSetClientView: NSView)

Informs the client view that `aRulerView` is about to be appropriated by `newClient`.

