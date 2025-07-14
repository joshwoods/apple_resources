

- Swift Charts
-  RulePlot 

Structure

# RulePlot

Chart content that represents a collection of data using a single horizontal or vertical rule.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct RulePlot
```

## Overview

Use `RulePlot` when you want to visualize data in the same way as with RuleMark, but you want to visualize an entire data collection with a single plot.

You can initialize and style the plot with simple values or key paths. Add modifiers with `KeyPath` before adding modifiers with simple values.

```
Chart {
    RulePlot(
        tasks,
        xStart: .value("Start time", \.startTime),
        xEnd: .value("End time", \.endTime),
        y: .value("Project", \.project)
    )
    .foregroundStyle(by: .value("Status", \.status))
    .opacity(/.opacity)
    .lineStyle(StrokeStyle(lineWidth: 8, lineCap: .round))
}
```

## Topics

### Plotting rules from a collection

init&lt;Data>(Data, x: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>, yStart: CGFloat?, yEnd: CGFloat?)

init&lt;Data, Y>(Data, x: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>, yStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>)

init&lt;Data>(Data, x: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>, yStart: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>, yEnd: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>)

init&lt;Data, Y>(Data, x: CGFloat?, yStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>)

init&lt;Data, Y>(Data, x: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>, yStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, Y>)

init&lt;Data>(Data, xStart: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>, xEnd: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>, y: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data>(Data, xStart: CGFloat?, xEnd: CGFloat?, y: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, y: KeyPath&lt;RulePlot&lt;Content>.DataElement, CGFloat>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, y: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;RulePlot&lt;Content>.DataElement, X>, y: CGFloat?)

### Supporting types

struct VectorizedRulePlotContent

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

struct BarPlot

Chart content that represents a collection of data using bars.

struct SectorPlot

Chart content that represents a collection of data using a sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

protocol VectorizedChartContent

A generic type that represents content conveyed via a chart.

