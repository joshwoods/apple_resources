

- Swift Charts
- VectorizedChartContent
-  symbolSize(\_:) 

Instance Method

# symbolSize(\_:)

Sets the plotting symbol size for the chart content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func symbolSize(_ size: KeyPath) -> some VectorizedChartContent
```

## Parameters 

`size`  

The symbol’s bounding box’s dimensions.

## See Also

### Setting symbol appearance

func symbol(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using different kinds of symbols.

func symbolSize(KeyPath&lt;Self.DataElement, CGFloat>) -> some VectorizedChartContent&lt;Self.DataElement> 

Sets the plotting symbol size for the chart content according to a perceived area.

