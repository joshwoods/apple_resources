

- Swift Charts
- ChartContent
-  offset(xStart:xEnd:yStart:yEnd:) 

Instance Method

# offset(xStart:xEnd:yStart:yEnd:)

Applies an offset to the chart content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func offset(
    xStart: CGFloat = 0,
    xEnd: CGFloat = 0,
    yStart: CGFloat = 0,
    yEnd: CGFloat = 0
) -> some ChartContent
```

## Parameters 

`xStart`  

The starting horizontal offset in screen coordinates.

`xEnd`  

The ending horizontal offset in screen coordinates.

`yStart`  

The starting vertical offset in screen coordinates.

`yEnd`  

The ending vertical offset in screen coordinates.

## Discussion

The `xStart`, `xEnd`, `yStart`, and `yEnd` offset values apply only to marks that have such properties, like bar marks and line segment marks.

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

func alignsMarkStylesWithPlotArea(Bool) -> some ChartContent

Aligns this item’s styles with the chart’s plot area.

