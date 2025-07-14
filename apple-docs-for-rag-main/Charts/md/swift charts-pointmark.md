

- Swift Charts
-  PointMark 

Structure

# PointMark

Chart content that represents data using points.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct PointMark
```

## Mentioned in 

Creating a chart using Swift Charts

## Overview

You can create different kinds of point charts using the `PointMark` chart content. One common chart you can build with point marks is a scatter plot which displays the relationship between two numerical data properties. To build a scatter plot use the `init(x:y:)`. Provide a `.value` for both the `x` and `y` parameters with a string, used as a label for the data, and the data element to be plotted. The following example plots the `wingLength` and `wingHeight` properties with x and y, respectively:

```
struct Insect {
    let name: String
    let family: String
    let wingLength: Double
    let wingWidth: Double
    let weight: Double
}

var data: [Insect] = [
    Insect(name: "Hepialidae", family: "Lepidoptera", wingLength: 61, wingWidth: 52, weight: 22),
    Insect(name: "Danaidae", family: "Lepidoptera", wingLength: 60, wingWidth: 48, weight: 24),
    Insect(name: "Riodinidae", family: "Lepidoptera", wingLength: 53, wingWidth: 43, weight: 18),
    // ...
]

var body: some View {
    Chart(data) {
        PointMark(
            x: .value("Wing Length", $0.wingLength),
            y: .value("Wing Width", $0.wingWidth)
        )
    }
}
```

### Adding Additional Data Fields

Swift Charts provides three additional modifiers for point mark that each allow you to plot an additional property to a unique visual channel.

| Modifier | Visual Channel |
|----|----|
| foregroundStyle(by:) | plot an additional property with color |
| symbol(by:) | plot an additional property with symbols |
| symbolSize(by:) | plot an additional property with size |

For example, to plot the `family` property from the previous example’s `Insect` structure as a color, add the foregroundStyle(by:) modifier:

```
Chart(data) {
    PointMark(
        x: .value("Wing Length", $0.wingLength),
        y: .value("Wing Width", $0.wingWidth)
    )
    .foregroundStyle(by: .value("Family", $0.family))
}
```

The foreground style modifier automatically generates a color scale that provides each mark with a color that reflects its value property. To learn how to modify the default color scale, see `ScaleModifiers`. The modifier also provides a default legend. To learn how to modify or disable the legend, see `ChartLegend`.

Alternatively, you can distinguish families with different symbols by plotting the `family` property using the symbol(by:) modifier:

```
Chart(data) {
    PointMark(
        x: .value("Wing Length", $0.wingLength),
        y: .value("Wing Length", $0.wingWidth)
    )
    .symbol(by: .value("Family", $0.family))
}
```

## Topics

### Creating a point mark

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>)

Creates a point mark that plots values to x and y.

### Initializers

init&lt;Y>(x: CGFloat?, y: PlottableValue&lt;Y>)

Creates a point mark with fixed x position and plots values with y.

init&lt;X>(x: PlottableValue&lt;X>, y: CGFloat?)

Creates a point mark that plots a value on x with fixed y position.

## Relationships

### Conforms To

- ChartContent
- Copyable
- Sendable

## See Also

### Marks

struct AreaMark

Chart content that represents data using the area of one or more regions.

struct LineMark

Chart content that represents data using a sequence of connected line segments.

struct RectangleMark

Chart content that represents data using rectangles.

struct RuleMark

Chart content that represents data using a single horizontal or vertical rule.

struct BarMark

Chart content that represents data using bars.

struct SectorMark

A sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

