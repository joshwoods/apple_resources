

- Swift Charts
- ChartContent
-  foregroundStyle(by:) 

Instance Method

# foregroundStyle(by:)

Represents data using a foreground style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func foregroundStyle(by value: PlottableValue) -> some ChartContent where D : Plottable
```

## Parameters 

`value`  

The data value to encode using foreground style.

## Mentioned in 

Creating a chart using Swift Charts

## See Also

### Encoding data into mark characteristics

func lineStyle&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using line styles.

func position&lt;P>(by: PlottableValue&lt;P>, axis: Axis?, span: MarkDimension) -> some ChartContent

Represents data using position.

func symbol&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using different kinds of symbols.

func symbolSize&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using symbol sizes.

