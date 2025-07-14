

- Swift Charts
- ChartContent
-  offset(\_:) 

Instance Method

# offset(\_:)

Applies an offset that you specify as a size to the chart content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func offset(_ value: CGSize) -> some ChartContent
```

## Parameters 

`value`  

The offset distance in screen coordinates.

## See Also

### Positioning marks

func offset(x: CGFloat, y: CGFloat) -> some ChartContent

Applies a vertical and horizontal offset to the chart content.

func offset(x: CGFloat, yStart: CGFloat, yEnd: CGFloat) -> some ChartContent

Applies an offset to the chart content.

func offset(xStart: CGFloat, xEnd: CGFloat, y: CGFloat) -> some ChartContent

Applies an offset to the chart content.

func offset(xStart: CGFloat, xEnd: CGFloat, yStart: CGFloat, yEnd: CGFloat) -> some ChartContent

Applies an offset to the chart content.

func alignsMarkStylesWithPlotArea(Bool) -> some ChartContent

Aligns this item’s styles with the chart’s plot area.

