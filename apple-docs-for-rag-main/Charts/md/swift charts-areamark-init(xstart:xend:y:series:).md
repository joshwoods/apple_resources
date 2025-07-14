

- Swift Charts
- AreaMark
-  init(xStart:xEnd:y:series:) 

Initializer

# init(xStart:xEnd:y:series:)

Creates an area mark that plots values with a horizontal interval and associates it with the specified series.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: PlottableValue,
    xEnd: PlottableValue,
    y: PlottableValue,
    series: PlottableValue
) where X : Plottable, Y : Plottable, S : Plottable
```

## Parameters 

`xStart`  

The starting horizontal position for the mark.

`xEnd`  

The ending horizontal position for the mark.

`y`  

The vertical position for the mark.

`series`  

A series to associate the mark with.

## Discussion

The initializer behaves like init(xStart:xEnd:y:), except that you can indicate which region each interval belongs to by providing a value for the `series` input. This enables you to plot more than one region on a single chart.

To plot a series of values that have a vertical interval, use init(x:yStart:yEnd:series:) instead.

## See Also

### Creating a range area chart

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates an area mark that plots values with a vertical interval.

init&lt;X, Y, S>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates an area mark that plots values with a vertical interval and associates it with the specified series.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>)

Creates an area mark that plots values with a horizontal interval.

