

- Swift Charts
- VectorizedChartContent
-  symbol(by:) 

Instance Method

# symbol(by:)

Represents data using different kinds of symbols.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func symbol(by value: PlottableProjection) -> some VectorizedChartContent
```

## Parameters 

`value`  

The data value. `value` must be categorial, such as `String`.

## See Also

### Setting symbol appearance

func symbolSize(KeyPath&lt;Self.DataElement, CGSize>) -> some VectorizedChartContent&lt;Self.DataElement> 

Sets the plotting symbol size for the chart content.

func symbolSize(KeyPath&lt;Self.DataElement, CGFloat>) -> some VectorizedChartContent&lt;Self.DataElement> 

Sets the plotting symbol size for the chart content according to a perceived area.

