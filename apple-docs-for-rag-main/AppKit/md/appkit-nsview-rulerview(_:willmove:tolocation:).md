

- AppKit
- NSView
-  rulerView(\_:willMove:toLocation:) 

Instance Method

# rulerView(\_:willMove:toLocation:)

Informs the client that `aRulerView` will move `aMarker`, an NSRulerMarker already on the ruler view.

macOS

``` source
@MainActor
func rulerView(
    _ ruler: NSRulerView,
    willMove marker: NSRulerMarker,
    toLocation location: CGFloat
) -> CGFloat
```

## Discussion

`location` is the marker’s tentative new location, expressed in the client view’s coordinate system. The value returned by the client view is actually used; the client can simply return `location` unchanged or adjust it as needed. For example, it may snap the location to a grid. This message is sent repeatedly to the client as the user drags the marker.

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

func rulerView(NSRulerView, willSetClientView: NSView)

Informs the client view that `aRulerView` is about to be appropriated by `newClient`.

