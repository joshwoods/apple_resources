

- Swift Charts
- AreaMark
-  init(x:yStart:yEnd:) 

Initializer

# init(x:yStart:yEnd:)

Creates an area mark that plots values with a vertical interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    yStart: PlottableValue,
    yEnd: PlottableValue
) where X : Plottable, Y : Plottable
```

## Parameters 

`x`  

The horizontal position for the mark.

`yStart`  

The starting vertical position for the mark.

`yEnd`  

The ending vertical position for the mark.

## Discussion

Use this initializer to create a range area chart with vertical intervals. For example you can create a region that encompasses all the temperatures over the course of a day, across a number of days:

```
Chart(data) { day in
    AreaMark(
        x: .value("Date", day.date),
        yStart: .value("Minimum Temperature", minimumTemperature),
        yEnd: .value("Maximum Temperature", day.maximumTemperature)
    )
}
```

If you want to plot values that have a horiztonal interval, use init(xStart:xEnd:y:) instead.

## See Also

### Creating a range area chart

init&lt;X, Y, S>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates an area mark that plots values with a vertical interval and associates it with the specified series.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>)

Creates an area mark that plots values with a horizontal interval.

init&lt;X, Y, S>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates an area mark that plots values with a horizontal interval and associates it with the specified series.

