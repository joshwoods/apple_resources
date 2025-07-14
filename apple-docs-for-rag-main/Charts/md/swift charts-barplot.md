

- Swift Charts
-  BarPlot 

Structure

# BarPlot

Chart content that represents a collection of data using bars.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct BarPlot
```

## Overview

Use `BarPlot` when you want to visualize data in the same way as with BarMark, but you want to visualize an entire data collection with a single plot.

You can initialize and style the plot with simple values or key paths. Add modifiers with `KeyPath` before adding modifiers with simple values.

```
BarPlot(
    votes,
    x: .value("Party", \.party),
    y: .value("Vote count", \.voteCount)
)
.foregroundStyle(by: \.partyShapeStyle)
.cornerRadius(4)
```

## Topics

### Plotting bars from a collection

init&lt;Data>(Data, x: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, width: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, height: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data, Y>(Data, x: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, yStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>, width: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>)

init&lt;Data>(Data, x: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, yStart: CGFloat?, yEnd: CGFloat?, width: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data>(Data, x: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, yStart: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, yEnd: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, width: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data>(Data, xStart: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, xEnd: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, y: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, height: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data>(Data, xStart: CGFloat?, xEnd: CGFloat?, y: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, height: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>, stacking: MarkStackingMethod)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, y: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, some Plottable>, height: MarkDimensions&lt;BarPlot&lt;Content>.DataElement>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, yStart: CGFloat?, yEnd: CGFloat?)

init&lt;Data, Y>(Data, xStart: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, xEnd: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, yStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, X>, yStart: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>, yEnd: KeyPath&lt;BarPlot&lt;Content>.DataElement, CGFloat>)

init&lt;Data, Y>(Data, xStart: CGFloat?, xEnd: CGFloat?, yStart: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;BarPlot&lt;Content>.DataElement, Y>)

### Supporting types

struct VectorizedBarPlotContent

An opaque vectorized chart content type.

## Relationships

### Conforms To

- ChartContent

  Conforms when `Content` conforms to `ChartContent`.

- Copyable
- VectorizedChartContent

  Conforms when `Content` conforms to `VectorizedChartContent`.

## See Also

### Vectorized plots

Creating a data visualization dashboard with Swift Charts

Visualize an entire data collection efficiently by instantiating a single vectorized plot in Swift Charts.

struct AreaPlot

Chart content that represents a function or a collection of data using the area of one or more regions.

struct LinePlot

Chart content that represents a function or a collection of data using a sequence of connected line segments.

struct PointPlot

Chart content that represents a collection of data using points.

struct RectanglePlot

Chart content that represents a collection of data using rectangles.

struct RulePlot

Chart content that represents a collection of data using a single horizontal or vertical rule.

struct SectorPlot

Chart content that represents a collection of data using a sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

protocol VectorizedChartContent

A generic type that represents content conveyed via a chart.

