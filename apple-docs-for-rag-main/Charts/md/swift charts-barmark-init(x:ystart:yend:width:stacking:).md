

- Swift Charts
- BarMark
-  init(x:yStart:yEnd:width:stacking:) 

Initializer

# init(x:yStart:yEnd:width:stacking:)

Creates a bar mark that plots a value on x with fixed y interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    x: PlottableValue,
    yStart: CGFloat? = nil,
    yEnd: CGFloat? = nil,
    width: MarkDimension = .automatic,
    stacking: MarkStackingMethod = .standard
) where X : Plottable
```

## Parameters 

`x`  

The value plotted with x.

`yStart`  

The y start position. If `yStart` is `nil` then the rectangle will start at the leading edge of the plotting area.

`yEnd`  

The y end position. If `yEnd` is `nil` then the rectangle will end at the trailing edge of the plotting area.

`width`  

The bar width. If `width` is `nil`, the default bar size will be applied.

`stacking`  

The stacking method for the bars with the same categorical/date values. If `stacking` is `nil`, the bars will not be stacked.

### Discussion

Use this initializer to create a chart with a single horizontal bar:

```
Chart(data) {
    BarMark(
        x: .value("Profit", $0.profit)
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

init&lt;Y>(xStart: CGFloat?, xEnd: CGFloat?, y: PlottableValue&lt;Y>, height: MarkDimension, stacking: MarkStackingMethod)

Creates a bar mark that plots values on y with fixed x interval.

