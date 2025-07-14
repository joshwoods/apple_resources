

- AppKit
- NSImageRep
-  draw(at:) 

Instance Method

# draw(at:)

Draws the image representation’s image data at the specified point in the current coordinate system.

macOS

``` source
func draw(at point: NSPoint) -> Bool
```

## Parameters 

`point`  

The point in the current coordinate system at which to draw the image.

## Return Value

true if the image was successfully drawn; otherwise, false. If the size of the image has not yet been set, this method returns false immediately

## Discussion

This method sets the origin of the current coordinate system to the specified point and then invokes the receiver’s `draw` method to draw the image at that point. Upon completion, it restores the current coordinates to their original setting. If `aPoint` is (0.0, 0.0), this method simply invokes the draw() method.

## See Also

### Drawing Images

func draw() -> Bool

Implemented by subclasses to draw the image in the current coordinate system.

func draw(in: NSRect) -> Bool

Draws the image, scaling it (as needed) to fit the specified rectangle.

func draw(in: NSRect, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat, respectFlipped: Bool, hints: [NSImageRep.HintKey : Any]?) -> Bool

Draws all or part of the image in the specified rectangle in the current coordinate system.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

