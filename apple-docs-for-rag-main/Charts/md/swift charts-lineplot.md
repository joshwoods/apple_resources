

- Swift Charts
-  LinePlot 

Structure

# LinePlot

Chart content that represents a function or a collection of data using a sequence of connected line segments.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct LinePlot
```

## Overview

Use `LinePlot` when you want to visualize data in the same way as with LineMark, but you want to plot a function or visualize an entire data collection with a single plot.

### Plotting lines from a collection

You can initialize and style the plot with simple values or key paths. Add modifiers with `KeyPath` before adding modifiers with simple values.

```
Chart {
    LinePlot(
        stocks,
        x: .value("Date", \.date),
        y: .value("Price", \.price),
        series: .value("Asset", \.symbol)
    )
    .foregroundStyle(by: .value("Asset", \.symbol))
}
```

### Plotting functions

In addition to providing data points, you can provide a function to a `LinePlot` to plot a function. For example, you can plot the function y = x^2 with:

```
Chart {
    LinePlot(x: "x", y: "y") { x in x * x }
}
.chartXScale(-10 ... 10)
.chartYScale(-10 ... 10)
```

You can add multiple function plots in a chart and use different foreground styles to distinguish among them.

```
Chart {
    LinePlot(x: "x", y: "y = sin(x)") { sin($0) }
        .foregroundStyle(by: .value("expression", "y=sin(x)"))
        .lineStyle(StrokeStyle(lineWidth: 5, lineCap: .round))
        .opacity(0.8)

    LinePlot(x: "x", y: "y = cos(x)") { cos($0) }
        .foregroundStyle(by: .value("expression", "y=cos(x)")
        .lineStyle(StrokeStyle(lineWidth: 5, lineCap: .round))
        .opacity(0.8)
}
.chartXScale(-10 ... 10)
.chartYScale(-10 ... 10)
```

You can plot a parametric function with the constructor with `x`, `y`, and `t`:

```
Chart {
    LinePlot(x: "x", y: "y", t: "t", domain: 0 ... .pi * 2) {
        t in (x: 10 * cos(5 * t) * cos(t), y: 10 * cos(5 * t) * sin(t))
    }
}
.chartXScale(domain: -10 ... 10)
.chartYScale(domain: -10 ... 10)
```

## Topics

### Plotting lines from a collection

init&lt;Data>(Data, x: PlottableProjection&lt;LinePlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;LinePlot&lt;Content>.DataElement, some Plottable>)

init&lt;Data>(Data, x: PlottableProjection&lt;LinePlot&lt;Content>.DataElement, some Plottable>, y: PlottableProjection&lt;LinePlot&lt;Content>.DataElement, some Plottable>, series: PlottableProjection&lt;LinePlot&lt;Content>.DataElement, some Plottable>)

### Supporting types

struct VectorizedLinePlotContent

An opaque vectorized chart content type.

struct FunctionLinePlotContent

### Initializers

init(x: LocalizedStringKey, y: LocalizedStringKey, domain: ClosedRange&lt;Double>?, function: (Double) -> Double)

Creates a mark that graphs a function y = f(x).

init&lt;S1, S2>(x: S1, y: S2, domain: ClosedRange&lt;Double>?, function: (Double) -> Double)

Creates a mark that graphs a function y = f(x).

init(x: Text, y: Text, domain: ClosedRange&lt;Double>?, function: (Double) -> Double)

Creates a mark that graphs a function y = f(x).

init&lt;S1, S2, S3>(x: S1, y: S2, t: S3, domain: ClosedRange&lt;Double>, function: (Double) -> (x: Double, y: Double))

Creates a mark that graphs a parametric function (x, y) = f(t).

init(x: Text, y: Text, t: Text, domain: ClosedRange&lt;Double>, function: (Double) -> (x: Double, y: Double))

Creates a mark that graphs a parametric function (x, y) = f(t).

init(x: LocalizedStringKey, y: LocalizedStringKey, t: LocalizedStringKey, domain: ClosedRange&lt;Double>, function: (Double) -> (x: Double, y: Double))

Creates a mark that graphs a parametric function (x, y) = f(t).

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

