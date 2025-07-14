

- Swift Charts
- LinePlot
-  init(\_:x:y:series:) 

Initializer

# init(\_:x:y:series:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    _ data: Data,
    x: PlottableProjection.DataElement, some Plottable>,
    y: PlottableProjection.DataElement, some Plottable>,
    series: PlottableProjection.DataElement, some Plottable>
) where Content == VectorizedLinePlotContent, Data : RandomAccessCollection
```

## See Also

### Plotting lines from a collection

init&lt;Data>(Data, x: PlottableProjection&lt;LinePlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;LinePlot&lt;Content>.DataElement, some Plottable>)

