

- AppKit
- NSImageRep
-  draw() 

Instance Method

# draw()

Implemented by subclasses to draw the image in the current coordinate system.

macOS

``` source
func draw() -> Bool
```

## Return Value

true if the image was successfully drawn; otherwise, false if there was a problem. The default version of this method simply returns true.

## Discussion

Subclass override this method to draw the image using the image data. By the time this method is called, the graphics state is already configured for you to draw the image at location (0.0, 0.0) in the current coordinate system.

The standard Application Kit subclasses all draw the image using the `NSCompositeCopy` composite operation defined in the `Constants` section of `NSImage`. Using the copy operator, the image data overwrites the destination without any blending effects. Transparent (alpha) regions in the source image appear black. To use other composite operations, you must place the representation into an `NSImage` object and use its draw(at:from:operation:fraction:) or draw(in:from:operation:fraction:) methods.

## See Also

### Drawing Images

func draw(at: NSPoint) -> Bool

Draws the image representation’s image data at the specified point in the current coordinate system.

func draw(in: NSRect) -> Bool

Draws the image, scaling it (as needed) to fit the specified rectangle.

func draw(in: NSRect, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat, respectFlipped: Bool, hints: [NSImageRep.HintKey : Any]?) -> Bool

Draws all or part of the image in the specified rectangle in the current coordinate system.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

