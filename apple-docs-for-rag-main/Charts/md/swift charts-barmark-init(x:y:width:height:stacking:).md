

- Swift Charts
- BarMark
-  init(x:y:width:height:stacking:) 

Initializer

# init(x:y:width:height:stacking:)

Creates a bar mark that plots values with x and y.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    y: PlottableValue,
    width: MarkDimension = .automatic,
    height: MarkDimension = .automatic,
    stacking: MarkStackingMethod = .standard
) where X : Plottable, Y : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`y`  

The value plotted with y.

`width`  

The bar width. If `width` is `nil`, the default bar size will be applied.

`height`  

The bar height. If `height` is `nil`, the default bar size will be applied.

`stacking`  

The stacking method for the bars with the same categorical/date values. If `stacking` is `nil`, the bars will not be stacked.

### Discussion

Use this initializer to create a chart with one or more bars. For horizontal bars, plot categories or dates with y and numbers with x. For vertical bars, plot categories or dates with x and numbers with y:

```
Chart(data) {
    BarMark(
        x: .value("Department", $0.department),
        y: .value("Profit", $0.profit)
    )
}
```

## See Also

### Creating a bar mark

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>, width: MarkDimension)

Creates a bar mark that plots values with x and its y interval.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, height: MarkDimension)

Creates a bar mark that plots values with its x interval and y.

init&lt;X>(x: PlottableValue&lt;X>, yStart: CGFloat?, yEnd: CGFloat?, width: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots a value on x with fixed y interval.

init&lt;Y>(xStart: CGFloat?, xEnd: CGFloat?, y: PlottableValue&lt;Y>, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values on y with fixed x interval.

