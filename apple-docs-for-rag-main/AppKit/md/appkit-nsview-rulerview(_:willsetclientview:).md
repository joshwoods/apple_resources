

- AppKit
- NSView
-  rulerView(\_:willSetClientView:) 

Instance Method

# rulerView(\_:willSetClientView:)

Informs the client view that `aRulerView` is about to be appropriated by `newClient`.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    willSetClientView newClient: NSView
)
```

## Discussion

The client view can use this opportunity to clear any cached information related to the ruler.

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

func rulerView(NSRulerView, shouldMove: NSRulerMarker) -> Bool

Requests permission for `aRulerView` to move `aMarker`.

func rulerView(NSRulerView, shouldRemove: NSRulerMarker) -> Bool

Requests permission for `aRulerView` to remove `aMarker`.

func rulerView(NSRulerView, willAdd: NSRulerMarker, atLocation: CGFloat) -> CGFloat

Informs the client that `aRulerView` will add the new NSRulerMarker, `aMarker`.

func rulerView(NSRulerView, willMove: NSRulerMarker, toLocation: CGFloat) -> CGFloat

Informs the client that `aRulerView` will move `aMarker`, an NSRulerMarker already on the ruler view.

