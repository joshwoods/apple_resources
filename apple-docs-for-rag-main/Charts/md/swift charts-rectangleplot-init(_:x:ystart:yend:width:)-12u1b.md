

- Swift Charts
- RectanglePlot
-  init(\_:x:yStart:yEnd:width:) 

Initializer

# init(\_:x:yStart:yEnd:width:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    _ data: Data,
    x: PlottableProjection.DataElement, some Plottable>,
    yStart: CGFloat? = nil,
    yEnd: CGFloat? = nil,
    width: MarkDimensions.DataElement> = .automatic
) where Content == VectorizedRectanglePlotContent, Data : RandomAccessCollection
```

## See Also

### Plotting rectangles from a collection

init&lt;Data>(Data, x: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, some Plottable>, width: MarkDimensions&lt;RectanglePlot&lt;Content>.DataElement>, height: MarkDimensions&lt;RectanglePlot&lt;Content>.DataElement>)

init&lt;Data, Y>(Data, x: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, some Plottable>, yStart: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, Y>, width: MarkDimensions&lt;RectanglePlot&lt;Content>.DataElement>)

init&lt;Data>(Data, x: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, some Plottable>, yStart: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, yEnd: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, width: MarkDimensions&lt;RectanglePlot&lt;Content>.DataElement>)

init&lt;Data>(Data, xStart: CGFloat?, xEnd: CGFloat?, y: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, some Plottable>, height: MarkDimensions&lt;RectanglePlot&lt;Content>.DataElement>)

init&lt;Data>(Data, xStart: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, xEnd: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, y: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, some Plottable>, height: MarkDimensions&lt;RectanglePlot&lt;Content>.DataElement>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, X>, y: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, some Plottable>, height: MarkDimensions&lt;RectanglePlot&lt;Content>.DataElement>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, X>, yStart: CGFloat?, yEnd: CGFloat?)

init&lt;Data, X, Y>(Data, xStart: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, X>, yStart: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, Y>)

init&lt;Data, Y>(Data, xStart: CGFloat?, xEnd: CGFloat?, yStart: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, Y>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, X>, yStart: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, yEnd: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>)

init&lt;Data, Y>(Data, xStart: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, xEnd: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, yStart: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RectanglePlot&lt;Content>.DataElement, Y>)

init&lt;Data>(Data, xStart: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, xEnd: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, yStart: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>, yEnd: KeyPath&lt;RectanglePlot&lt;Content>.DataElement, CGFloat>)

