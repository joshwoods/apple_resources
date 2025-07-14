

- SwiftUI
- ImagePaint
-  init(image:sourceRect:scale:) 

Initializer

# init(image:sourceRect:scale:)

Creates a shape-filling shape style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    image: Image,
    sourceRect: CGRect = CGRect(x: 0, y: 0, width: 1, height: 1),
    scale: CGFloat = 1
)
```

## Parameters 

`image`  

The image to be drawn.

`sourceRect`  

A unit-space rectangle defining how much of the source image to draw. The results are undefined if `sourceRect` selects areas outside the `[0, 1]` range in either axis.

`scale`  

A scale factor applied to the image during rendering.

