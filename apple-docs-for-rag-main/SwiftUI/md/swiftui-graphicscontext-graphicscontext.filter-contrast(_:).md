

- SwiftUI
- GraphicsContext
- GraphicsContext.Filter
-  contrast(\_:) 

Type Method

# contrast(\_:)

Returns a filter that applies a contrast adjustment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func contrast(_ amount: Double) -> GraphicsContext.Filter
```

## Parameters 

`amount`  

An amount to adjust the contrast. A value of zero leaves the result completely gray. A value of one leaves the result unchanged. You can use values greater than one.

## Return Value

A filter that applies a contrast adjustment.

## Discussion

This filter is equivalent to the `contrast` filter primitive defined by the Scalable Vector Graphics (SVG) specification.

## See Also

### Changing brightness and contrast

static func brightness(Double) -> GraphicsContext.Filter

Returns a filter that applies a brightness adjustment.

