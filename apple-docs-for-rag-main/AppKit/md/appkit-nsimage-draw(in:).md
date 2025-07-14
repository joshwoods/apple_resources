

- AppKit
- NSImage
-  draw(in:) 

Instance Method

# draw(in:)

Draws the image in the specified rectangle.

macOS 10.9+

``` source
func draw(in rect: NSRect)
```

## Parameters 

`rect`  

The rectangle in which to draw the image, specified in the current coordinate system.

## Discussion

This method draws the entire image in the specified rectangle, scaling the image as needed. The method composites the image using the NSCompositeSourceOver operation

## See Also

### Drawing Images

func draw(at: NSPoint, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat)

Draws all or part of the image at the specified point in the current coordinate system.

func draw(in: NSRect, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat)

Draws all or part of the image in the specified rectangle in the current coordinate system.

func draw(in: NSRect, from: NSRect, operation: NSCompositingOperation, fraction: CGFloat, respectFlipped: Bool, hints: [NSImageRep.HintKey : Any]?)

Draws all or part of the image in the specified rectangle respecting the hints and the orientation of the current coordinate system.

func drawRepresentation(NSImageRep, in: NSRect) -> Bool

Draws the image using the specified image representation object.

enum NSCompositingOperation

Constants that describe compositing operators in terms of source and destination images, each having an opaque and transparent region.

