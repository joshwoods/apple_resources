

- Swift Charts
- VectorizedChartContent
-  foregroundStyle(by:) 

Instance Method

# foregroundStyle(by:)

Represents data using a foreground style.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func foregroundStyle(by value: PlottableProjection) -> some VectorizedChartContent
```

## Parameters 

`value`  

The data value to encode using foreground style.

## See Also

### Encoding data into mark characteristics

func lineStyle(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using line styles.

func symbol(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using different kinds of symbols.

func symbolSize(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using symbol sizes.

