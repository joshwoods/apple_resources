

- Swift Charts
-  ChartContent 

Protocol

# ChartContent

A type that represents the content that you draw on a chart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
protocol ChartContent
```

## Overview

You build a Chart by adding instances that conform to the `ChartContent` protocol to the chart’s `content` closure. The following example adds three explicit BarMark instances to a chart:

```
Chart {
    BarMark(
        x: .value("Shape Type", "Cube"),
        y: .value("Total Count", 5)
    )
    BarMark(
        x: .value("Shape Type", "Sphere"),
        y: .value("Total Count", 6)
    )
    BarMark(
        x: .value("Shape Type", "Pyramid"),
        y: .value("Total Count", 4)
    )
}
```

The chart draws marks that correspond to the instances that you specify:

You can combine any number of marks or types of marks in a single chart by listing them individually as shown in the above example, wrapping them in a ForEach, or any combination of these. For some mark types, like LineMark, you can group the marks into series using the mark’s `series` initialization parameter.

### Configure chart content

The `ChartContent` protocol provides a set of modifiers that you use to configure the properties of chart content. These behave like SwiftUI view modifiers, except that they act on chart content rather than views. Any of the types that conform to the protocol can use these modifiers. For example, you can add the foregroundStyle(_:) modifier to the bar representing the number of spheres in the previous example to make it red:

```
BarMark(
    x: .value("Shape Type", "Sphere"),
    y: .value("Total Count", 6)
)
.foregroundStyle(.red)
```

## Topics

### Styling marks

func foregroundStyle&lt;S>(S) -> some ChartContent

Sets the foreground style for the chart content.

func opacity(Double) -> some ChartContent

Sets the opacity for the chart content.

func cornerRadius(CGFloat, style: RoundedCornerStyle) -> some ChartContent

Sets the corner radius of the chart content.

func lineStyle(StrokeStyle) -> some ChartContent

Sets the style for line marks.

func interpolationMethod(InterpolationMethod) -> some ChartContent

Plots line and area marks with the interpolation method that you specify.

### Positioning marks

func offset(CGSize) -> some ChartContent

Applies an offset that you specify as a size to the chart content.

func offset(x: CGFloat, y: CGFloat) -> some ChartContent

Applies a vertical and horizontal offset to the chart content.

func offset(x: CGFloat, yStart: CGFloat, yEnd: CGFloat) -> some ChartContent

Applies an offset to the chart content.

func offset(xStart: CGFloat, xEnd: CGFloat, y: CGFloat) -> some ChartContent

Applies an offset to the chart content.

func offset(xStart: CGFloat, xEnd: CGFloat, yStart: CGFloat, yEnd: CGFloat) -> some ChartContent

Applies an offset to the chart content.

func alignsMarkStylesWithPlotArea(Bool) -> some ChartContent

Aligns this item’s styles with the chart’s plot area.

### Setting symbol appearance

func symbol&lt;S>(S) -> some ChartContent

Sets a plotting symbol type for the chart content.

func symbol&lt;V>(symbol: () -> V) -> some ChartContent

Sets a SwiftUI view to use as the symbol for the chart content.

func symbolSize(CGSize) -> some ChartContent

Sets the plotting symbol size for the chart content.

func symbolSize(CGFloat) -> some ChartContent

Sets the plotting symbol size for the chart content according to a perceived area.

### Encoding data into mark characteristics

func foregroundStyle&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using a foreground style.

func lineStyle&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using line styles.

func position&lt;P>(by: PlottableValue&lt;P>, axis: Axis?, span: MarkDimension) -> some ChartContent

Represents data using position.

func symbol&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using different kinds of symbols.

func symbolSize&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using symbol sizes.

### Annotating marks

func annotation&lt;C>(position: AnnotationPosition, alignment: Alignment, spacing: CGFloat?, content: () -> C) -> some ChartContent

Annotates this mark or collection of marks with a view positioned relative to its bounds.

func annotation&lt;C>(position: AnnotationPosition, alignment: Alignment, spacing: CGFloat?, content: (AnnotationContext) -> C) -> some ChartContent

Annotates this mark or collection of marks with a view positioned relative to its bounds.

### Masking and clipping

func mask&lt;C>(content: () -> C) -> some ChartContent

Masks chart content using the alpha channel of the specified content.

func clipShape(some Shape, style: FillStyle) -> some ChartContent

Sets a clip shape for the chart content.

### Configuring accessibility

func accessibilityHidden(Bool) -> some ChartContent

Specifies whether to hide this chart content from system accessibility features.

func accessibilityIdentifier(String) -> some ChartContent

Adds an identifier string to the chart content.

func accessibilityLabel(LocalizedStringKey) -> some ChartContent

Adds a label to the chart content that describes its contents.

func accessibilityLabel&lt;S>(S) -> some ChartContent

Adds a label to the chart content that describes its contents.

func accessibilityLabel(Text) -> some ChartContent

Adds a label to the chart content that describes its contents.

func accessibilityValue(LocalizedStringKey) -> some ChartContent

Adds a description of the value that the chart content contains.

func accessibilityValue&lt;S>(S) -> some ChartContent

Adds a description of the value that the chart content contains.

func accessibilityValue(Text) -> some ChartContent

Adds a description of the value that the chart content contains.

### Implementing chart content

var body: Self.Body

The content and behavior of the chart content.

**Required**

associatedtype Body : ChartContent

The type of chart content contained in the body of this instance.

**Required**

### Supporting types

struct AnyChartContent

A type-erased chart content.

### Instance Methods

func annotation&lt;C>(position: AnnotationPosition, alignment: Alignment, spacing: CGFloat?, overflowResolution: AnnotationOverflowResolution, content: () -> C) -> some ChartContent

Annotates this mark or collection of marks with a view positioned relative to its bounds.

func annotation&lt;C>(position: AnnotationPosition, alignment: Alignment, spacing: CGFloat?, overflowResolution: AnnotationOverflowResolution, content: (AnnotationContext) -> C) -> some ChartContent

Annotates this mark or collection of marks with a view positioned relative to its bounds.

func blur(radius: CGFloat) -> some ChartContent

Applies a Gaussian blur to this chart content.

func compositingLayer() -> some ChartContent

func compositingLayer&lt;V>(style: (PlaceholderContentView&lt;Self>) -> V) -> some ChartContent

func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> some ChartContent

A chart content that adds a shadow to this chart content.

func zIndex(Double) -> some ChartContent

Controls the display order of overlapping chart content.

## Relationships

### Inherited By

- VectorizedChartContent

### Conforming Types

- AnyChartContent
- AreaMark
- AreaPlot

  Conforms when `Content` conforms to `ChartContent`.

- BarMark
- BarPlot

  Conforms when `Content` conforms to `ChartContent`.

- BuilderConditional

  Conforms when `TrueContent` conforms to `ChartContent` and `FalseContent` conforms to `ChartContent`.

- FunctionAreaPlotContent
- FunctionLinePlotContent
- LineMark
- LinePlot

  Conforms when `Content` conforms to `ChartContent`.

- Plot

  Conforms when `Content` conforms to `ChartContent`.

- PointMark
- PointPlot

  Conforms when `Content` conforms to `ChartContent`.

- RectangleMark
- RectanglePlot

  Conforms when `Content` conforms to `ChartContent`.

- RuleMark
- RulePlot

  Conforms when `Content` conforms to `ChartContent`.

- SectorMark
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

### Charts

Creating a chart using Swift Charts

Make a chart by combining chart building blocks in SwiftUI.

Visualizing your app’s data

Build complex and interactive charts using Swift Charts.

struct Chart

A SwiftUI view that displays a chart.

struct ChartContentBuilder

A result builder that you use to compose the contents of a chart.

struct Plot

A mechanism for grouping chart contents into a single entity.

