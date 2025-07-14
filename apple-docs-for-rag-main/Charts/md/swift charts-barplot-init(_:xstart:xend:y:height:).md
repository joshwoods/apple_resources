

- Swift Charts
- BarPlot
-  init(\_:xStart:xEnd:y:height:) 

Initializer

# init(\_:xStart:xEnd:y:height:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    _ data: Data,
    xStart: PlottableProjection.DataElement, X>,
    xEnd: PlottableProjection.DataElement, X>,
    y: PlottableProjection.DataElement, some Plottable>,
    height: MarkDimensions.DataElement> = .automatic
) where Content == VectorizedBarPlotContent, Data : RandomAccessCollection, X : Plottable
```

## See Also

### Plotting bars from a collection

init&lt;Data>(Data, x: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, width: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, height: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data, Y>(Data, x: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, yStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>, width: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>)

init&lt;Data>(Data, x: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, yStart: CGFloat?, yEnd: CGFloat?, width: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data>(Data, x: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, yStart: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, yEnd: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, width: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data>(Data, xStart: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, xEnd: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, y: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, height: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data>(Data, xStart: CGFloat?, xEnd: CGFloat?, y: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, height: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, yStart: CGFloat?, yEnd: CGFloat?)

init&lt;Data, Y>(Data, xStart: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, xEnd: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, yStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, yStart: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, yEnd: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>)

init&lt;Data, Y>(Data, xStart: CGFloat?, xEnd: CGFloat?, yStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>)

