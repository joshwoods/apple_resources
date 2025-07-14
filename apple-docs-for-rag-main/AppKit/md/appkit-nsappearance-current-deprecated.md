

- AppKit
- NSAppearance
-  current Deprecated

Type Property

# current

Returns the appearance object that’s active on the current thread.

macOS 10.9–12.0Deprecated

``` source
class var current: NSAppearance! { get set }
```

Deprecated

Use performAsCurrentDrawingAppearance(_:) to temporarily set the drawing appearance, or currentDrawingAppearance to access the current drawing appearance.

## Return Value

The appearance object that’s set on the current thread.

## Discussion

When a UI element draws to the screen, it automatically sets its appearance object to the active appearance on the current thread.

## See Also

### Getting and Setting the Current Appearance

class func currentDrawing() -> NSAppearance

The appearance that the system uses for color and asset resolution, and that’s active for drawing, usually from locking focus on a view.

func performAsCurrentDrawingAppearance(() -> Void)

Sets the appearance to be the active drawing appearance and perform the specified block.

