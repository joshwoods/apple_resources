

- Swift Charts
- LineMark
-  init(x:y:series:) 

Initializer

# init(x:y:series:)

Creates a separate line for each unique value of series.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    y: PlottableValue,
    series: PlottableValue
) where X : Plottable, Y : Plottable, S : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`y`  

The value plotted with y.

`series`  

The value with which to split the line series by.

### Discussion

Use this initializer to create a multi-line chart from a single data source.

```
Chart(sunshineData) {
    LineMark(
        x: .value("Month", $0.date),
        y: .value("Hours of Sunshine", $0.hoursOfSunshine)
    )
    .foregroundStyle(by: .value("City", $0.city))
}
```

## See Also

### Creating a line mark

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>)

Creates a line mark.

