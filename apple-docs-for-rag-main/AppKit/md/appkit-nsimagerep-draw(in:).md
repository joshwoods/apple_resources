

- AppKit
- NSImageRep
-  draw(in:) 

Instance Method

# draw(in:)

Draws the image, scaling it (as needed) to fit the specified rectangle.

macOS

``` source
func draw(in rect: NSRect) -> Bool
```

## Parameters 

`rect`  

The rectangle in the current coordinate system in which to draw the image.

## Return Value

true if the image was successfully drawn; otherwise, false. If the size of the image has not yet been set, this method returns false immediately.

## Discussion

This method sets the origin of the current coordinate system to the origin of the specified rectangle before invoking the receiver’s draw() method. If the rectangle size is different from the image’s native size, this method adjusts the coordinate transform, causing the image to be scaled appropriately. After the `draw` method returns, the coordinate system changes are undone, restoring the original graphics state.

## See Also

### Drawing Images

func draw() -> Bool

Implemented by subclasses to draw the image in the current coordinate system.

func draw(at: NSPoint) -> Bool

Draws the image representation’s image data at the specified point in the current coordinate system.

func draw(in: NSRect, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat, respectFlipped: Bool, hints: [NSImageRep.HintKey : Any]?) -> Bool

Draws all or part of the image in the specified rectangle in the current coordinate system.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

