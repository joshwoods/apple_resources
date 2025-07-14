

- Swift Charts
- ChartContent
-  alignsMarkStylesWithPlotArea(\_:) 

Instance Method

# alignsMarkStylesWithPlotArea(\_:)

Aligns this item’s styles with the chart’s plot area.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func alignsMarkStylesWithPlotArea(_ aligns: Bool = true) -> some ChartContent
```

## Parameters 

`aligns`  

A Boolean value that indicates whether to align this item’s styles with the plotting area.

## Discussion

Marks map unit-point coordinates within the plot area’s bounds.

## See Also

### Positioning marks

func offset(CGSize) -> some ChartContent

Applies an offset that you specify as a size to the chart content.

func offset(x: CGFloat, y: CGFloat) -> some ChartContent

Applies a vertical and horizontal offset to the chart content.

func offset(x: CGFloat, yStart: CGFloat, yEnd: CGFloat) -> some ChartContent

Applies an offset to the chart content.

func offset(xStart: CGFloat, xEnd: CGFloat, y: CGFloat) -> some ChartContent

Applies an offset to the chart content.

func offset(xStart: CGFloat, xEnd: CGFloat, yStart: CGFloat, yEnd: CGFloat) -> some ChartContent

Applies an offset to the chart content.

