

- Swift Charts
- ChartContent
-  symbol(by:) 

Instance Method

# symbol(by:)

Represents data using different kinds of symbols.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func symbol(by value: PlottableValue) -> some ChartContent where D : Plottable
```

## Parameters 

`value`  

The data value. `value` must be categorial, such as `String`.

## See Also

### Encoding data into mark characteristics

func foregroundStyle&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using a foreground style.

func lineStyle&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using line styles.

func position&lt;P>(by: PlottableValue&lt;P>, axis: Axis?, span: MarkDimension) -> some ChartContent

Represents data using position.

func symbolSize&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using symbol sizes.

