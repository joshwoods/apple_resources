

- SwiftUI
- GraphicsContext
- GraphicsContext.Shading
-  tiledImage(\_:origin:sourceRect:scale:) 

Type Method

# tiledImage(\_:origin:sourceRect:scale:)

Returns a shading instance that tiles an image across the infinite plane.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func tiledImage(
    _ image: Image,
    origin: CGPoint = .zero,
    sourceRect: CGRect = CGRect(x: 0, y: 0, width: 1, height: 1),
    scale: CGFloat = 1
) -> GraphicsContext.Shading
```

## Parameters 

`image`  

An Image to use as fill.

`origin`  

The point in the current user space where SwiftUI places the bottom left corner of the part of the image defined by `sourceRect`. The image repeats as needed.

`sourceRect`  

A unit space subregion of the image. The default is a unit rectangle, which selects the whole image.

`scale`  

A factor that you can use to control the image size.

## Return Value

A shading instance filled with a tiled image.

