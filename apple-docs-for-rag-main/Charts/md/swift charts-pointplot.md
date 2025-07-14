

- Swift Charts
-  PointPlot 

Structure

# PointPlot

Chart content that represents a collection of data using points.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct PointPlot
```

## Overview

Use `PointPlot` when you want to visualize data in the same way as with PointMark, but you want to visualize an entire data collection with a single plot.

You can initialize and style the plot with simple values or key paths. Add modifiers with `KeyPath` before adding modifiers with simple values.

```
Chart {
    PointPlot(
        flightDelays,
        x: .value("Flight Distance", \.distance),
        y: .value("Flight Delay", \.delay)
    )
    .foregroundStyle(by: .value("Airline", \.airline))
    .opacity(\.opacity)
    .symbolSize(by: .value("Capacity", \.passengerCount))
    .symbol(.circle)
}
```

## Topics

### Plotting points from a collection

init&lt;Data>(Data, x: KeyPath&lt;Data.Element, CGFloat>, y: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data>(Data, x: CGFloat?, y: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data>(Data, x: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>, y: CGFloat?)

init&lt;Data>(Data, x: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data>(Data, x: PlottableProjection&lt;PointPlot&lt;Content>.DataElement, some Plottable>, y: KeyPath&lt;PointPlot&lt;Content>.DataElement, CGFloat>)

### Supporting types

struct VectorizedPointPlotContent

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

struct RectanglePlot

Chart content that represents a collection of data using rectangles.

struct RulePlot

Chart content that represents a collection of data using a single horizontal or vertical rule.

struct BarPlot

Chart content that represents a collection of data using bars.

struct SectorPlot

Chart content that represents a collection of data using a sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

protocol VectorizedChartContent

A generic type that represents content conveyed via a chart.

