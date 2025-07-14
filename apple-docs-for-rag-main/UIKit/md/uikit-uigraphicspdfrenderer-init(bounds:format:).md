

- UIKit
- UIGraphicsPDFRenderer
-  init(bounds:format:) 

Initializer

# init(bounds:format:)

Creates a new graphics renderer with the specified bounds and format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
init(
    bounds: CGRect,
    format: UIGraphicsPDFRendererFormat
)
```

## Parameters 

`bounds`  

The bounds of the Core Graphics context available to the renderer, with values in points.

`format`  

A UIGraphicsPDFRendererFormat object that encapsulates the format applied to the renderer’s context.

## Return Value

An initialized PDF graphics renderer.

## Discussion

Use this initializer to create a PDF renderer when you want to override the default format for the current device. Otherwise, use the init(bounds:) method present on the abstract superclass, UIGraphicsRenderer.

