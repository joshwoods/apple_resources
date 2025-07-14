

- UIKit
- UIGraphicsRenderer
-  init(bounds:) 

Initializer

# init(bounds:)

Creates a new graphics renderer with the specified bounds and a default format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
convenience init(bounds: CGRect)
```

## Parameters 

`bounds`  

The bounds of the Core Graphics context available to the renderer, with values measured in points.

## Return Value

An initialized graphics renderer.

## Discussion

Use this initializer to create a graphics renderer that operates on Core Graphics contexts with the specified bounds. This initializer uses the default() static method on UIGraphicsRendererFormat to create the renderer’s format, thereby selecting parameters that are the most appropriate for the current device.

## See Also

### Initializing a graphics renderer

init(bounds: CGRect, format: UIGraphicsRendererFormat)

Creates a new graphics renderer with the given bounds and format.

