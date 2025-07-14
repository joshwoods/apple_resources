

- Swift Charts
-  SectorPlot 

Structure

# SectorPlot

Chart content that represents a collection of data using a sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct SectorPlot
```

## Overview

Use `SectorPlot` when you want to visualize data in the same way as with SectorMark, but you want to visualize an entire data collection with a single plot.

You can initialize and style the plot with simple values or key paths. Add modifiers with `KeyPath` before adding modifiers with simple values.

```
SectorPlot(
    votes,
    angle: .value("Vote count", \.voteCount),
    angularInset: 1
)
.foregroundStyle(by: .value("Party", \.party))
.cornerRadius(4)
```

## Topics

### Plotting sectors from a collection

init&lt;Data>(Data, angle: PlottableProjection&lt;SectorPlot&lt;Content>.DataElement, some Plottable>, innerRadius: MarkDimensions&lt;SectorPlot&lt;Content>.DataElement>, outerRadius: MarkDimensions&lt;SectorPlot&lt;Content>.DataElement>, angularInset: CGFloat?)

init&lt;Data>(Data, angle: PlottableProjection&lt;SectorPlot&lt;Content>.DataElement, some Plottable>, innerRadius: MarkDimensions&lt;SectorPlot&lt;Content>.DataElement>, outerRadius: MarkDimensions&lt;SectorPlot&lt;Content>.DataElement>, angularInset: KeyPath&lt;SectorPlot&lt;Content>.DataElement, CGFloat>)

### Supporting types

struct VectorizedSectorPlotContent

An opaque vectorized chart content type.

## Relationships

### Conforms To

- ChartContent

  Conforms when `Content` conforms to `VectorizedChartContent`.

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

struct BarPlot

Chart content that represents a collection of data using bars.

protocol VectorizedChartContent

A generic type that represents content conveyed via a chart.

