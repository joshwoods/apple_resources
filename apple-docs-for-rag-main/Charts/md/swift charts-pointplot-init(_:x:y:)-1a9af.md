

- Swift Charts
- PointPlot
-  init(\_:x:y:) 

Initializer

# init(\_:x:y:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    _ data: Data,
    x: KeyPath,
    y: PlottableProjection.DataElement, some Plottable>
) where Content == VectorizedPointPlotContent, Data : RandomAccessCollection
```

## See Also

### Plotting points from a collection

init&lt;Data>(Data, x: CGFloat?, y: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data>(Data, x: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>, y: CGFloat?)

init&lt;Data>(Data, x: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data>(Data, x: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>, y: KeyPath&lt;PointPlot&lt;Content>.DataElement, CGFloat>)

