

- Swift Charts
- RulePlot
-  init(\_:xStart:xEnd:y:) 

Initializer

# init(\_:xStart:xEnd:y:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    _ data: Data,
    xStart: CGFloat? = nil,
    xEnd: CGFloat? = nil,
    y: PlottableProjection.DataElement, some Plottable>
) where Content == VectorizedRulePlotContent, Data : RandomAccessCollection
```

## See Also

### Plotting rules from a collection

init&lt;Data>(Data, x: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>, yStart: CGFloat?, yEnd: CGFloat?)

init&lt;Data, Y>(Data, x: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>, yStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>)

init&lt;Data>(Data, x: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>, yStart: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>, yEnd: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>)

init&lt;Data, Y>(Data, x: CGFloat?, yStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>)

init&lt;Data, Y>(Data, x: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>, yStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>)

init&lt;Data>(Data, xStart: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>, xEnd: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>, y: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, y: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, y: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, y: CGFloat?)

