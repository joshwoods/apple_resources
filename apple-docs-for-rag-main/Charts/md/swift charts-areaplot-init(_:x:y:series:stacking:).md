

- Swift Charts
- AreaPlot
-  init(\_:x:y:series:stacking:) 

Initializer

# init(\_:x:y:series:stacking:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    _ data: Data,
    x: PlottableProjection.DataElement, some Plottable>,
    y: PlottableProjection.DataElement, some Plottable>,
    series: PlottableProjection.DataElement, some Plottable>,
    stacking: MarkStackingMethod = .standard
) where Content == VectorizedAreaPlotContent, Data : RandomAccessCollection
```

## See Also

### Plotting areas from a collection

init&lt;Data>(Data, x: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, stacking: MarkStackingMethod)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, X>, y: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, X>, y: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, series: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data, Y>(Data, x: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, yStart: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, Y>)

init&lt;Data, Y>(Data, x: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, yStart: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, Y>, series: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>)

