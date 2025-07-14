

- UIKit
- UIGraphicsRenderer
-  init(bounds:format:) 

Initializer

# init(bounds:format:)

Creates a new graphics renderer with the given bounds and format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
init(
    bounds: CGRect,
    format: UIGraphicsRendererFormat
)
```

## Parameters 

`bounds`  

The bounds of the Core Graphics context available to the renderer, with values measured in points.

`format`  

The format applied to the renderer’s context. This object is an instance of the subclass of UIGraphicsRendererFormat appropriate for the concrete subclass of `UIGraphicsRenderer` you are using.

## Return Value

An initialized graphics renderer.

## Discussion

Use this initializer to create a graphics renderer when you want to override the default format for the current device.

The format instance is copied at initialization time, so you can immediately reuse the same instance to create additional renderers.

## See Also

### Initializing a graphics renderer

convenience init(bounds: CGRect)

Creates a new graphics renderer with the specified bounds and a default format.

