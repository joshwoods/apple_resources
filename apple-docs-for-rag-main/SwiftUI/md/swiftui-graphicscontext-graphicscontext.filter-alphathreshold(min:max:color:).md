

- SwiftUI
- GraphicsContext
- GraphicsContext.Filter
-  alphaThreshold(min:max:color:) 

Type Method

# alphaThreshold(min:max:color:)

Returns a filter that replaces each pixel with alpha components within a range by a constant color, or transparency otherwise.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func alphaThreshold(
    min: Double,
    max: Double = 1,
    color: Color = Color.black
) -> GraphicsContext.Filter
```

## Parameters 

`min`  

The minimum alpha threshold. Pixels whose alpha component is less than this value will render as transparent. Results are undefined unless `min 

`max`  

The maximum alpha threshold. Pixels whose alpha component is greater than this value will render as transparent. Results are undefined unless `min 

`color`  

The color that is output for pixels with an alpha component between the two threshold values.

## Return Value

A filter that applies a threshold to alpha values.

## See Also

### Adjusting opacity

static var luminanceToAlpha: GraphicsContext.Filter

Returns a filter that sets the opacity of each pixel based on its luminance.

