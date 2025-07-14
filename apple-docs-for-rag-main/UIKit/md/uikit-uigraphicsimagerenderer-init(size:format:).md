

- UIKit
- UIGraphicsImageRenderer
-  init(size:format:) 

Initializer

# init(size:format:)

Creates an image renderer with the specified size and format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
init(
    size: CGSize,
    format: UIGraphicsImageRendererFormat
)
```

## Parameters 

`size`  

The size of images output from the renderer, specified in points.

`format`  

A UIGraphicsImageRendererFormat object that encapsulates the format used to create the renderer context.

## Return Value

An initialized renderer.

## Discussion

Use this initializer to create an image renderer when you want to override the default format for the current device. Provide the size of the images you want to create, and an instance of UIGraphicsImageRendererFormat with the required configuration.

## See Also

### Initializing an image renderer

init(bounds: CGRect, format: UIGraphicsImageRendererFormat)

Creates an image renderer with the specified bounds and format.

convenience init(size: CGSize)

Creates an image renderer for drawing images of the specified size.

