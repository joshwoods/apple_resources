

- Swift Charts
- ChartContent
-  symbolSize(\_:) 

Instance Method

# symbolSize(\_:)

Sets the plotting symbol size for the chart content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func symbolSize(_ size: CGSize) -> some ChartContent
```

## Parameters 

`size`  

The symbol’s bounding box’s dimensions.

## See Also

### Setting symbol appearance

func symbol&lt;S>(S) -> some ChartContent

Sets a plotting symbol type for the chart content.

func symbol&lt;V>(symbol: () -> V) -> some ChartContent

Sets a SwiftUI view to use as the symbol for the chart content.

func symbolSize(CGFloat) -> some ChartContent

Sets the plotting symbol size for the chart content according to a perceived area.

