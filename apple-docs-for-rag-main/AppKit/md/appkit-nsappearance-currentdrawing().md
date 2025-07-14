

- AppKit
- NSAppearance
-  currentDrawing() 

Type Method

# currentDrawing()

The appearance that the system uses for color and asset resolution, and that’s active for drawing, usually from locking focus on a view.

macOS 11.0+

``` source
class func currentDrawing() -> NSAppearance
```

## Return Value

The current appearance used for drawing.

## See Also

### Getting and Setting the Current Appearance

func performAsCurrentDrawingAppearance(() -> Void)

Sets the appearance to be the active drawing appearance and perform the specified block.

class var current: NSAppearance!

Returns the appearance object that’s active on the current thread.

Deprecated

