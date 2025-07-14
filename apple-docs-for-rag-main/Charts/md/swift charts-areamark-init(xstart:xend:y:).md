

- Swift Charts
- AreaMark
-  init(xStart:xEnd:y:) 

Initializer

# init(xStart:xEnd:y:)

Creates an area mark that plots values with a horizontal interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: PlottableValue,
    xEnd: PlottableValue,
    y: PlottableValue
) where X : Plottable, Y : Plottable
```

## Parameters 

`xStart`  

The starting horizontal position for the mark.

`xEnd`  

The ending horizontal position for the mark.

`y`  

The vertical position for the mark.

## Discussion

Use this initializer to create a range area chart with horizontal intervals. For example you can create a region that encompasses all the temperatures over the course of a day, across a number of days:

```
Chart(data) { day in
    AreaMark(
        xStart: .value("Minimum Temperature", minimumTemperature),
        xEnd: .value("Maximum Temperature", day.maximumTemperature),
        y: .value("Date", day.date)
    )
}
```

If you want to plot values that have a vertical interval, use init(x:yStart:yEnd:) instead.

## See Also

### Creating a range area chart

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates an area mark that plots values with a vertical interval.

init&lt;X, Y, S>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates an area mark that plots values with a vertical interval and associates it with the specified series.

init&lt;X, Y, S>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates an area mark that plots values with a horizontal interval and associates it with the specified series.

