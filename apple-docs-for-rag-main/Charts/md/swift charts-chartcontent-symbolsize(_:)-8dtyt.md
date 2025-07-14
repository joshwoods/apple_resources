

- Swift Charts
- ChartContent
-  symbolSize(\_:) 

Instance Method

# symbolSize(\_:)

Sets the plotting symbol size for the chart content according to a perceived area.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func symbolSize(_ area: CGFloat) -> some ChartContent
```

## Parameters 

`area`  

The perceived area in square points. For example, a square with 10 points on each side has an area of 100 square points.

## See Also

### Setting symbol appearance

func symbol&lt;S>(S) -> some ChartContent

Sets a plotting symbol type for the chart content.

func symbol&lt;V>(symbol: () -> V) -> some ChartContent

Sets a SwiftUI view to use as the symbol for the chart content.

func symbolSize(CGSize) -> some ChartContent

Sets the plotting symbol size for the chart content.

