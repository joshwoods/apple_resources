

- Swift Charts
- VectorizedChartContent
-  lineStyle(by:) 

Instance Method

# lineStyle(by:)

Represents data using line styles.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func lineStyle(by value: PlottableProjection) -> some VectorizedChartContent
```

## Parameters 

`value`  

The keyPath accessor for the data value that encodes the line style.

## See Also

### Encoding data into mark characteristics

func foregroundStyle(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using a foreground style.

func symbol(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using different kinds of symbols.

func symbolSize(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using symbol sizes.

