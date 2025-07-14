

- SwiftUI
- ShapeStyle
-  image(\_:sourceRect:scale:) 

Type Method

# image(\_:sourceRect:scale:)

A shape style that fills a shape by repeating a region of an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func image(
    _ image: Image,
    sourceRect: CGRect = CGRect(x: 0, y: 0, width: 1, height: 1),
    scale: CGFloat = 1
) -> ImagePaint
```

Available when `Self` is `ImagePaint`.

## Parameters 

`image`  

The image to be drawn.

`sourceRect`  

A unit-space rectangle defining how much of the source image to draw. The results are undefined if `sourceRect` selects areas outside the `[0, 1]` range in either axis.

`scale`  

A scale factor applied to the image during rendering.

## Discussion

For information about how to use shape styles, see ShapeStyle.

