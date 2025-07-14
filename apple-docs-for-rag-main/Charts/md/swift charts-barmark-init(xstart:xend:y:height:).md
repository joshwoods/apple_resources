

- Swift Charts
- BarMark
-  init(xStart:xEnd:y:height:) 

Initializer

# init(xStart:xEnd:y:height:)

Creates a bar mark that plots values with its x interval and y.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: PlottableValue,
    xEnd: PlottableValue,
    y: PlottableValue,
    height: MarkDimension = .automatic
) where X : Plottable, Y : Plottable
```

## Parameters 

`xStart`  

The value plotted with x start.

`xEnd`  

The value plotted with x end.

`y`  

The value plotted with y.

`height`  

The bar height. If `height` is `nil`, the default bar size will be applied.

### Discussion

Use this initializer to show horizontal intervals for one or more categories:

```
Chart(data) {
   BarMark(
       xStart: .value("Start Time", $0.start),
       xEnd: .value("End Time", $0.end),
       y: .value("Job", $0.job)
   )
}
```

## See Also

### Creating a bar mark

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>, width: MarkDimension)

Creates a bar mark that plots values with x and its y interval.

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, width: MarkDimension, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values with x and y.

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, width: MarkDimension, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values with x and y.

init&lt;X>(x: PlottableValue&lt;X>, yStart: CGFloat?, yEnd: CGFloat?, width: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots a value on x with fixed y interval.

init&lt;Y>(xStart: CGFloat?, xEnd: CGFloat?, y: PlottableValue&lt;Y>, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values on y with fixed x interval.

