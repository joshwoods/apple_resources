

- Swift Charts
- AreaMark
-  init(x:y:stacking:) 

Initializer

# init(x:y:stacking:)

Creates an area mark using the specified horizontal and vertical positions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    y: PlottableValue,
    stacking: MarkStackingMethod = .standard
) where X : Plottable, Y : Plottable
```

## Parameters 

`x`  

The horizontal position for the mark.

`y`  

The vertical position for the mark.

`stacking`  

The way in which the chart stacks area regions. The default is standard.

## Discussion

You can use this initializer to create a basic area chart:

```
Chart(cheeseburgerCost) { cost in
    AreaMark(
        x: .value("Date", cost.date),
        y: .value("Price", cost.price)
    )
}
```

The resulting chart automatically scales and labels the axes based on the data, and fills the area under the data points with a default color:

## See Also

### Creating an area mark

init&lt;X, Y, S>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, series: PlottableValue&lt;S>, stacking: MarkStackingMethod)

Creates an area mark and associates it with the specified series.

