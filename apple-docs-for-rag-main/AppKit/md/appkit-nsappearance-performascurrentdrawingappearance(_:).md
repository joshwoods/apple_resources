

- AppKit
- NSAppearance
-  performAsCurrentDrawingAppearance(\_:) 

Instance Method

# performAsCurrentDrawingAppearance(\_:)

Sets the appearance to be the active drawing appearance and perform the specified block.

macOS 11.0+

``` source
func performAsCurrentDrawingAppearance(_ block: () -> Void)
```

## Parameters 

`block`  

The block to invoke after setting the appearance to be the current drawing appearance.

## Discussion

This method saves and restores the previous current appearance.

## See Also

### Getting and Setting the Current Appearance

class func currentDrawing() -> NSAppearance

The appearance that the system uses for color and asset resolution, and that’s active for drawing, usually from locking focus on a view.

class var current: NSAppearance!

Returns the appearance object that’s active on the current thread.

Deprecated

