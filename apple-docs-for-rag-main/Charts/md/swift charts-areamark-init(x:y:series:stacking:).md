

- Swift Charts
- AreaMark
-  init(x:y:series:stacking:) 

Initializer

# init(x:y:series:stacking:)

Creates an area mark and associates it with the specified series.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    y: PlottableValue,
    series: PlottableValue,
    stacking: MarkStackingMethod = .standard
) where X : Plottable, Y : Plottable, S : Plottable
```

## Parameters 

`x`  

The horizontal position for the mark.

`y`  

The vertical position for the mark.

`series`  

A series to associate the mark with.

`stacking`  

The way in which the chart stacks area regions. The default is standard.

## Discussion

The initializer behaves like init(x:y:stacking:), except that you can indicate which region each data point belongs to by providing a value for the `series` input. This enables you to plot more than one region on a single chart.

## See Also

### Creating an area mark

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, stacking: MarkStackingMethod)

Creates an area mark using the specified horizontal and vertical positions.

