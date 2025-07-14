

- UIKit
- UIGraphicsImageRenderer
-  init(bounds:format:) 

Initializer

# init(bounds:format:)

Creates an image renderer with the specified bounds and format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
init(
    bounds: CGRect,
    format: UIGraphicsImageRendererFormat
)
```

## Parameters 

`bounds`  

The bounds of the image context the image renderer creates and subsequently draws upon. Specify values in points in the Core Graphics coordinate space.

`format`  

A UIGraphicsImageRendererFormat object that encapsulates the format used to create the renderer context.

## Return Value

An initialized image renderer.

## Discussion

Use this initializer to create an image renderer when you want to override the default format for the current device.

## See Also

### Initializing an image renderer

convenience init(size: CGSize)

Creates an image renderer for drawing images of the specified size.

init(size: CGSize, format: UIGraphicsImageRendererFormat)

Creates an image renderer with the specified size and format.

