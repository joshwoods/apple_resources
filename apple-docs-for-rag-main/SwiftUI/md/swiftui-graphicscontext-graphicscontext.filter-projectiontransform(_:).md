

- SwiftUI
- GraphicsContext
- GraphicsContext.Filter
-  projectionTransform(\_:) 

Type Method

# projectionTransform(\_:)

Returns a filter that that transforms the rasterized form of subsequent graphics primitives.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func projectionTransform(_ matrix: ProjectionTransform) -> GraphicsContext.Filter
```

## Parameters 

`matrix`  

A projection transform to apply to the rasterized form of graphics primitives.

## Return Value

A filter that applies a transform.

