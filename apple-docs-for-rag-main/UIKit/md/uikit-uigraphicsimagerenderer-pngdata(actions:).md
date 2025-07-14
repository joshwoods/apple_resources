

- UIKit
- UIGraphicsImageRenderer
-  pngData(actions:) 

Instance Method

# pngData(actions:)

Creates a PNG-encoded image from a set of drawing instructions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func pngData(actions: (UIGraphicsImageRendererContext) -> Void) -> Data
```

## Parameters 

`actions`  

A UIGraphicsImageRenderer.DrawingActions block that, when invoked by the renderer, executes a set of drawing instructions to create the output image.

## Return Value

A Data object representing a PNG-encoded representation of the image created by the supplied drawing actions.

## Discussion

You provide a set of drawing instructions as the block argument to this method, and the method returns the resulting image as a PNG-encoded Data object.

You can call this method repeatedly to create multiple images, each of which has identical dimensions and format.

## See Also

### Creating images

func image(actions: (UIGraphicsImageRendererContext) -> Void) -> UIImage

Creates an image from a set of drawing instructions.

func jpegData(withCompressionQuality: CGFloat, actions: (UIGraphicsImageRendererContext) -> Void) -> Data

Creates a JPEG-encoded image from a set of drawing instructions.

typealias DrawingActions

A closure for drawing an image.

