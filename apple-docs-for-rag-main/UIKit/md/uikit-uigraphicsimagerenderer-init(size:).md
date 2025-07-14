

- UIKit
- UIGraphicsImageRenderer
-  init(size:) 

Initializer

# init(size:)

Creates an image renderer for drawing images of the specified size.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
convenience init(size: CGSize)
```

## Parameters 

`size`  

The size of images output from the renderer, specified in points.

## Return Value

An initialized image renderer.

## Discussion

Use this initializer to create an image renderer that will draw images of a given size. This renderer uses the default() static method on UIGraphicsImageRendererContext to create its context, thereby selecting parameters that are the most appropriate for the current device.

## See Also

### Initializing an image renderer

init(bounds: CGRect, format: UIGraphicsImageRendererFormat)

Creates an image renderer with the specified bounds and format.

init(size: CGSize, format: UIGraphicsImageRendererFormat)

Creates an image renderer with the specified size and format.

