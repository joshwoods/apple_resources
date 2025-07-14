

- Swift Charts
- BarMark
-  init(x:yStart:yEnd:width:) 

Initializer

# init(x:yStart:yEnd:width:)

Creates a bar mark that plots values with x and its y interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    yStart: PlottableValue,
    yEnd: PlottableValue,
    width: MarkDimension = .automatic
) where X : Plottable, Y : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`yStart`  

The value plotted with y start.

`yEnd`  

The value plotted with y end.

`width`  

The bar width. If `width` is `nil`, the default bar size will be applied.

### Discussion

Use this initializer to show vertical intervals for one or more categories:

```
Chart(data) {
   BarMark(
       x: .value("Job", $0.job),
       yStart: .value("Start Time", $0.start),
       yEnd: .value("End Time", $0.end)
   )
}
```

## See Also

### Creating a bar mark

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, height: MarkDimension)

Creates a bar mark that plots values with its x interval and y.

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, width: MarkDimension, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values with x and y.

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, width: MarkDimension, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values with x and y.

init&lt;X>(x: PlottableValue&lt;X>, yStart: CGFloat?, yEnd: CGFloat?, width: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots a value on x with fixed y interval.

init&lt;Y>(xStart: CGFloat?, xEnd: CGFloat?, y: PlottableValue&lt;Y>, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values on y with fixed x interval.

