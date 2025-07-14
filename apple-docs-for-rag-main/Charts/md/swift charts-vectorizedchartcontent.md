

- Swift Charts
-  VectorizedChartContent 

Protocol

# VectorizedChartContent

A generic type that represents content conveyed via a chart.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol VectorizedChartContent : ChartContent
```

## Overview

Its primary associated type represents the data element, sometimes called *data point*, *observation* or *aggregate*.

Usually, `DataElement` has properties to determine visual attributes directly, or indirectly by encoding `Plottable` values through a chart scale.

## Topics

### Styling marks

func foregroundStyle(KeyPath&lt;Self.DataElement, some ShapeStyle>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using a foreground style.

func opacity(KeyPath&lt;Self.DataElement, CGFloat>) -> some VectorizedChartContent&lt;Self.DataElement> 

func lineStyle(KeyPath&lt;Self.DataElement, StrokeStyle>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using line styles.

func position(by: PlottableProjection&lt;Self.DataElement, some Plottable>, axis: Axis?, span: MarkDimension) -> some VectorizedChartContent&lt;Self.DataElement> 

### Setting symbol appearance

func symbol(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using different kinds of symbols.

func symbolSize(KeyPath&lt;Self.DataElement, CGSize>) -> some VectorizedChartContent&lt;Self.DataElement> 

Sets the plotting symbol size for the chart content.

func symbolSize(KeyPath&lt;Self.DataElement, CGFloat>) -> some VectorizedChartContent&lt;Self.DataElement> 

Sets the plotting symbol size for the chart content according to a perceived area.

### Encoding data into mark characteristics

func foregroundStyle(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using a foreground style.

func lineStyle(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using line styles.

func symbol(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using different kinds of symbols.

func symbolSize(by: PlottableProjection&lt;Self.DataElement, some Plottable>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using symbol sizes.

### Configuring accessibility

func accessibilityHidden(KeyPath&lt;Self.DataElement, Bool>) -> some VectorizedChartContent&lt;Self.DataElement> 

Specifies whether to hide this chart content from system accessibility features.

func accessibilityIdentifier(KeyPath&lt;Self.DataElement, String>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds an identifier string to the chart content.

func accessibilityLabel(KeyPath&lt;Self.DataElement, some StringProtocol>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a label to the chart content that describes its contents.

func accessibilityValue(KeyPath&lt;Self.DataElement, some StringProtocol>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a description of the value that the chart content contains.

### Supporting types

struct PlottableProjection

### Associated Types

associatedtype DataElement

**Required**

### Instance Methods

func accessibilityLabel(KeyPath&lt;Self.DataElement, Text>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a label to the chart content that describes its contents.

func accessibilityLabel(KeyPath&lt;Self.DataElement, LocalizedStringKey>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a label to the chart content that describes its contents.

func accessibilityValue(KeyPath&lt;Self.DataElement, LocalizedStringKey>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a description of the value that the chart content contains.

func accessibilityValue(KeyPath&lt;Self.DataElement, Text>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a description of the value that the chart content contains.

## Relationships

### Inherits From

- ChartContent

### Conforming Types

- AreaPlot

  Conforms when `Content` conforms to `VectorizedChartContent`.

- BarPlot

  Conforms when `Content` conforms to `VectorizedChartContent`.

- LinePlot

  Conforms when `Content` conforms to `VectorizedChartContent`.

- PointPlot

  Conforms when `Content` conforms to `VectorizedChartContent`.

- RectanglePlot

  Conforms when `Content` conforms to `VectorizedChartContent`.

- RulePlot

  Conforms when `Content` conforms to `VectorizedChartContent`.

- SectorPlot

  Conforms when `Content` conforms to `VectorizedChartContent`.

- VectorizedAreaPlotContent
- VectorizedBarPlotContent
- VectorizedLinePlotContent
- VectorizedPointPlotContent
- VectorizedRectanglePlotContent
- VectorizedRulePlotContent
- VectorizedSectorPlotContent

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

struct SectorPlot

Chart content that represents a collection of data using a sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

