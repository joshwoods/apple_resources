

- SwiftUI
- GraphicsContext
-  addFilter(\_:options:) 

Instance Method

# addFilter(\_:options:)

Adds a filter that applies to subsequent drawing operations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func addFilter(
    _ filter: GraphicsContext.Filter,
    options: GraphicsContext.FilterOptions = FilterOptions()
)
```

## Parameters 

`filter`  

A graphics context filter that you create by calling one of the GraphicsContext.Filter factory methods.

`options`  

A set of options from GraphicsContext.FilterOptions that you can use to configure filter operations.

## Discussion

To draw with filtering, SwiftUI:

- Rasterizes the drawing operation to an implicit transparency layer without blending, adjusting opacity, or applying any clipping.

- Applies the filter to the layer containing the rasterized image.

- Composites the layer onto the background, using the context’s current blend mode, opacity setting, and clip shapes.

When SwiftUI draws with a filter, the blend mode might apply to regions outside the drawing operation’s intrinsic shape, but inside its clip shape. That might result in unexpected behavior for certain blend modes like copy, where the drawing operation completely overwrites the background even if the source alpha is zero.

## See Also

### Filtering

struct Filter

A type that applies image processing operations to rendered content.

struct FilterOptions

Options that configure a filter that you add to a graphics context.

struct BlurOptions

Options that configure the graphics context filter that creates blur.

struct ShadowOptions

Options that configure the graphics context filter that creates shadows.

