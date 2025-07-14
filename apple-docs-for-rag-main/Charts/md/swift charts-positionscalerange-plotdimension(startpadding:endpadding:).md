

- Swift Charts
- PositionScaleRange
-  plotDimension(startPadding:endPadding:) 

Type Method

# plotDimension(startPadding:endPadding:)

A scale range that fills the plot area with the given padding values at start and end, respectively.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func plotDimension(
    startPadding: CGFloat = 0,
    endPadding: CGFloat = 0
) -> PlotDimensionScaleRange
```

Available when `Self` is `PlotDimensionScaleRange`.

## Parameters 

`startPadding`  

The start padding value in screen coordinates.

`endPadding`  

The end padding value in screen coordinates.

