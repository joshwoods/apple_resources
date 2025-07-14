

- Swift Charts
-  AreaPlot 

Structure

# AreaPlot

Chart content that represents a function or a collection of data using the area of one or more regions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct AreaPlot
```

## Overview

Use `AreaPlot` when you want to visualize data in the same way as with AreaMark, but you want to plot a function or visualize an entire data collection with a single plot.

### Plotting areas from a collection

You can initialize and style the plot with simple values or key paths. Add modifiers with `KeyPath` before adding modifiers with simple values.

```
Chart {
    AreaPlot(
        portfolioElements,
        x: .value("Date", \.date),
        y: .value("Asset value", \.assetValue),
        series: .value("Asset", \.asset),
        stacking: .standard
    )
    .foregroundStyle(by: .value("Asset", \.asset))
}
```

### Plotting functions

In addition to providing data points, you can provide a function to an `AreaPlot` to plot a function. For example, you can plot the area between y = x and y = x^2 - 1 with:

```
Chart {
    AreaPlot(x: "x", yStart: "x", yEnd: "x^2 - 1") { x in (yStart: x, yEnd: x * x - 1) }
}
.chartXScale(domain: -2 ... 2)
.chartYScale(domain: -4 ... 4)
```

You can also provide a single function to an `AreaPlot`. In this case it will plot the area between zero and the given function.

```
Chart {
    AreaPlot(x: "x", y: "x^2 - 1") { x in x * x - 1 }
}
.chartXScale(domain: -2 ... 2)
.chartYScale(domain: -4 ... 4)
```

## Topics

### Plotting areas from a collection

init&lt;Data>(Data, x: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, stacking: MarkStackingMethod)

init&lt;Data>(Data, x: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, series: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, stacking: MarkStackingMethod)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, X>, y: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data, X>(Data, xStart: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, X>, xEnd: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, X>, y: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, series: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data, Y>(Data, x: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, yStart: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, Y>)

init&lt;Data, Y>(Data, x: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>, yStart: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, Y>, yEnd: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, Y>, series: PlottableProjection&lt;AreaPlot&lt;Content>.DataElement, some Plottable>)

### Supporting types

struct VectorizedAreaPlotContent

An opaque vectorized chart content type.

struct FunctionAreaPlotContent

### Initializers

init(x: Text, y: Text, domain: ClosedRange&lt;Double>?, function: (Double) -> Double)

Creates a mark that fills the area between zero and the given function.

init&lt;S1, S2>(x: S1, y: S2, domain: ClosedRange&lt;Double>?, function: (Double) -> Double)

Creates a mark that fills the area between zero and the given function.

init(x: LocalizedStringKey, y: LocalizedStringKey, domain: ClosedRange&lt;Double>?, function: (Double) -> Double)

Creates a mark that fills the area between zero and the given function.

init&lt;S1, S2, S3>(x: S1, yStart: S2, yEnd: S3, domain: ClosedRange&lt;Double>?, function: (Double) -> (yStart: Double, yEnd: Double))

Creates a mark that fills the area between two functions (yStart, yEnd) = f(x).

init(x: LocalizedStringKey, yStart: LocalizedStringKey, yEnd: LocalizedStringKey, domain: ClosedRange&lt;Double>?, function: (Double) -> (yStart: Double, yEnd: Double))

Creates a mark that fills the area between two functions (yStart, yEnd) = f(x).

init(x: Text, yStart: Text, yEnd: Text, domain: ClosedRange&lt;Double>?, function: (Double) -> (yStart: Double, yEnd: Double))

Creates a mark that fills the area between two functions (yStart, yEnd) = f(x).

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

struct SectorPlot

Chart content that represents a collection of data using a sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

protocol VectorizedChartContent

A generic type that represents content conveyed via a chart.

