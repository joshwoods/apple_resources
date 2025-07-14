

- Swift Charts
- BarMark
-  init(xStart:xEnd:y:height:stacking:) 

Initializer

# init(xStart:xEnd:y:height:stacking:)

Creates a bar mark that plots values on y with fixed x interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    xStart: CGFloat? = nil,
    xEnd: CGFloat? = nil,
    y: PlottableValue,
    height: MarkDimension = .automatic,
    stacking: MarkStackingMethod = .standard
) where Y : Plottable
```

## Parameters 

`xStart`  

The x start position. If `xStart` is `nil` then the rectangle will start at the leading edge of the plotting area.

`xEnd`  

The x end position. If `xStart` is `nil` then the rectangle will end at the trailing edge of the plotting area.

`y`  

The value plotted with y.

`height`  

The bar height. If `height` is `nil`, the default bar size will be applied.

`stacking`  

The stacking method for the bars with the same categorical/date values. If `stacking` is `nil`, the bars will not be stacked.

### Discussion

Use this initializer to create a chart with a single vertical bar:

```
Chart(data) {
    BarMark(
        y: .value("Profit", $0.profit)
    )
    .foregroundStyle(by: .value("Product Category", $0.productCategory))
}
```

## See Also

### Creating a bar mark

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>, width: MarkDimension)

Creates a bar mark that plots values with x and its y interval.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, height: MarkDimension)

Creates a bar mark that plots values with its x interval and y.

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, width: MarkDimension, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values with x and y.

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, width: MarkDimension, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values with x and y.

init&lt;X>(x: PlottableValue&lt;X>, yStart: CGFloat?, yEnd: CGFloat?, width: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots a value on x with fixed y interval.

