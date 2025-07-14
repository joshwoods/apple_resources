

- Swift Charts
- LineMark
-  init(x:y:) 

Initializer

# init(x:y:)

Creates a line mark.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    y: PlottableValue
) where X : Plottable, Y : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`y`  

The value plotted with y.

### Discussion

Use this initializer to create a chart with a single line.

```
Chart(sunshineData) {
    LineMark(
        x: .value("Month", $0.date),
        y: .value("Hours of Sunshine", $0.hoursOfSunshine)
    )
}
```

## See Also

### Creating a line mark

init&lt;X, Y, S>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates a separate line for each unique value of series.

