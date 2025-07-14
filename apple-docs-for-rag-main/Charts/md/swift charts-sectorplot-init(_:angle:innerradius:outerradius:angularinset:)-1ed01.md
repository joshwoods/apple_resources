

- Swift Charts
- SectorPlot
-  init(\_:angle:innerRadius:outerRadius:angularInset:) 

Initializer

# init(\_:angle:innerRadius:outerRadius:angularInset:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    _ data: Data,
    angle: PlottableProjection.DataElement, some Plottable>,
    innerRadius: MarkDimensions.DataElement> = .automatic,
    outerRadius: MarkDimensions.DataElement> = .automatic,
    angularInset: CGFloat? = nil
) where Content == VectorizedSectorPlotContent, Data : RandomAccessCollection
```

## See Also

### Plotting sectors from a collection

init&lt;Data>(Data, angle: PlottableProjection&lt;SectorPlot&lt;Content>.DataElement, some Plottable>, innerRadius: MarkDimensions&lt;SectorPlot&lt;Content>.DataElement>, outerRadius: MarkDimensions&lt;SectorPlot&lt;Content>.DataElement>, angularInset: KeyPath&lt;SectorPlot&lt;Content>.DataElement, CGFloat>)

