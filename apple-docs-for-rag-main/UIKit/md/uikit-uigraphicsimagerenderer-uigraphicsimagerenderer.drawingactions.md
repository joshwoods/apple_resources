

- UIKit
- UIGraphicsImageRenderer
-  UIGraphicsImageRenderer.DrawingActions 

Type Alias

# UIGraphicsImageRenderer.DrawingActions

A closure for drawing an image.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
typealias DrawingActions = (UIGraphicsImageRendererContext) -> Void
```

## Discussion

`UIGraphicsImageDrawingActions` defines a block type that takes a UIGraphicsImageRendererContext object as an argument and has no return value.

You provide a block of this type as an argument to the image drawing methods on UIGraphicsImageRenderer. Your block should use the provided image renderer context to perform the drawing operations you want the renderer to execute.

See Creating an image with an image renderer for an example use of a `UIGraphicsImageDrawingActions` block.

## See Also

### Creating images

func image(actions: (UIGraphicsImageRendererContext) -> Void) -> UIImage

Creates an image from a set of drawing instructions.

func jpegData(withCompressionQuality: CGFloat, actions: (UIGraphicsImageRendererContext) -> Void) -> Data

Creates a JPEG-encoded image from a set of drawing instructions.

func pngData(actions: (UIGraphicsImageRendererContext) -> Void) -> Data

Creates a PNG-encoded image from a set of drawing instructions.

