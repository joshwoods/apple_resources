

- AppKit
- NSImage
-  draw(in:from:operation:fraction:) 

Instance Method

# draw(in:from:operation:fraction:)

Draws all or part of the image in the specified rectangle in the current coordinate system.

macOS

``` source
func draw(
    in rect: NSRect,
    from fromRect: NSRect,
    operation op: NSCompositingOperation,
    fraction delta: CGFloat
)
```

## Parameters 

`rect`  

The rectangle in which to draw the image, specified in the current coordinate system.

`fromRect`  

The source rectangle specifying the portion of the image you want to draw. The coordinates of this rectangle must be specified using the image’s own coordinate system. If you pass in `NSZeroRect`, the entire image is drawn.

`op`  

The compositing operation to use when drawing the image. See the NSCompositingOperation constants.

`delta`  

The opacity of the image, specified as a value from 0.0 to 1.0. Specifying a value of 0.0 draws the image as fully transparent while a value of 1.0 draws the image as fully opaque. Values greater than 1.0 are interpreted as 1.0.

## Discussion

If the `srcRect` and `dstRect` rectangles have different sizes, the source portion of the image is scaled to fit the specified destination rectangle. The image is otherwise positioned and oriented using the current coordinate system.

Unlike the compositeToPoint:fromRect:operation: and compositeToPoint:fromRect:operation:fraction: methods, this method checks the rectangle you pass to the `srcRect` parameter and makes sure it does not lie outside the image bounds.

## See Also

### Drawing Images

func draw(in: NSRect)

Draws the image in the specified rectangle.

func draw(at: NSPoint, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat)

Draws all or part of the image at the specified point in the current coordinate system.

func draw(in: NSRect, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat, respectFlipped: Bool, hints: [NSImageRep.HintKey : Any]?)

Draws all or part of the image in the specified rectangle respecting the hints and the orientation of the current coordinate system.

func drawRepresentation(NSImageRep, in: NSRect) -> Bool

Draws the image using the specified image representation object.

enum NSCompositingOperation

Constants that describe compositing operators in terms of source and destination images, each having an opaque and transparent region.

