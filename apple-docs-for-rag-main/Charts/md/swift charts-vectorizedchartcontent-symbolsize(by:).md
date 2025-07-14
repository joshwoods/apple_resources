

- Swift Charts
- VectorizedChartContent
-  symbolSize(by:) 

Instance Method

# symbolSize(by:)

Represents data using symbol sizes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func symbolSize(by value: PlottableProjection) -> some VectorizedChartContent
```

## Parameters 

`value`  

The data value to encode by size.

## See Also

### Encoding data into mark characteristics

func foregroundStyle(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using a foreground style.

func lineStyle(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using line styles.

func symbol(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using different kinds of symbols.

