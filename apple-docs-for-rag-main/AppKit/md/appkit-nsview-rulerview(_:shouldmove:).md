

- AppKit
- NSView
-  rulerView(\_:shouldMove:) 

Instance Method

# rulerView(\_:shouldMove:)

Requests permission for `aRulerView` to move `aMarker`.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    shouldMove marker: NSRulerMarker
) -> Bool
```

## Discussion

If the client returns true the ruler view allows the user to move the marker; if the client returns false the marker doesn’t move.

The user’s ability to move a marker is typically set on the marker itself, using NSRulerMarker’s isMovable method. You should use this client view method only when the marker’s movability can vary depending on a variable condition (for example, if graphic items can be locked down to prevent them from being inadvertently moved).

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

func rulerView(NSRulerView, shouldAdd: NSRulerMarker) -> Bool

Requests permission for `aRulerView` to add `aMarker`, an NSRulerMarker being dragged onto the ruler by the user.

func rulerView(NSRulerView, shouldRemove: NSRulerMarker) -> Bool

Requests permission for `aRulerView` to remove `aMarker`.

func rulerView(NSRulerView, willAdd: NSRulerMarker, atLocation: CGFloat) -> CGFloat

Informs the client that `aRulerView` will add the new NSRulerMarker, `aMarker`.

func rulerView(NSRulerView, willMove: NSRulerMarker, toLocation: CGFloat) -> CGFloat

Informs the client that `aRulerView` will move `aMarker`, an NSRulerMarker already on the ruler view.

func rulerView(NSRulerView, willSetClientView: NSView)

Informs the client view that `aRulerView` is about to be appropriated by `newClient`.

