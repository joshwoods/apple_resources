

- Swift Charts
- AreaMark
-  init(x:yStart:yEnd:series:) 

Initializer

# init(x:yStart:yEnd:series:)

Creates an area mark that plots values with a vertical interval and associates it with the specified series.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    yStart: PlottableValue,
    yEnd: PlottableValue,
    series: PlottableValue
) where X : Plottable, Y : Plottable, S : Plottable
```

## Parameters 

`x`  

The horizontal position for the mark.

`yStart`  

The starting vertical position for the mark.

`yEnd`  

The ending vertical position for the mark.

`series`  

A series to associate the mark with.

## Discussion

The initializer behaves like init(x:yStart:yEnd:), except that you can indicate which region each interval belongs to by providing a value for the `series` input. This enables you to plot more than one region on a single chart.

To plot a series of values that have a horizontal interval, use init(xStart:xEnd:y:series:) instead.

## See Also

### Creating a range area chart

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates an area mark that plots values with a vertical interval.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>)

Creates an area mark that plots values with a horizontal interval.

init&lt;X, Y, S>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates an area mark that plots values with a horizontal interval and associates it with the specified series.

