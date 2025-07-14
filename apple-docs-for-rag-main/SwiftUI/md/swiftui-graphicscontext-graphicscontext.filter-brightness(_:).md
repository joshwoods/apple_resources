

- SwiftUI
- GraphicsContext
- GraphicsContext.Filter
-  brightness(\_:) 

Type Method

# brightness(\_:)

Returns a filter that applies a brightness adjustment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func brightness(_ amount: Double) -> GraphicsContext.Filter
```

## Parameters 

`amount`  

An amount to add to the pixel’s color components.

## Return Value

A filter that applies a brightness adjustment.

## Discussion

This filter is different than `brightness` filter primitive defined by the Scalable Vector Graphics (SVG) specification. You can obtain an effect like that filter using a grayscale(_:) color multiply. However, this filter does match the CIColorControls filter’s brightness adjustment.

## See Also

### Changing brightness and contrast

static func contrast(Double) -> GraphicsContext.Filter

Returns a filter that applies a contrast adjustment.

