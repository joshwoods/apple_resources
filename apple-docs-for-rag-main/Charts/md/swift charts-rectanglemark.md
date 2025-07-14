

- Swift Charts
-  RectangleMark 

Structure

# RectangleMark

Chart content that represents data using rectangles.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct RectangleMark
```

## Overview

Use rectangle mark to map data fields to rectangles. You can use the rectangle mark to create heat map charts or to annotate rectangular areas in a chart.

### Create a Heat Map with Rectangle Marks

When presenting data about the effectiveness of a machine learning model, you typically organize the data using a confusion matrix which shows the predicted versus the actual results of the model. To create a 2D heat map that represents a machine learning model you use init(x:y:width:height:). The example below uses a 2D heat map to visualize a basic confusion matrix with the following layout:

|              | Negative       | Positive       |
|--------------|----------------|----------------|
| **Negative** | True Negative  | False Negative |
| **Positive** | False Positive | True Positive  |

The number of records in each cell, `num`, is represented by the color of its corresponding rectangle. This is done by applying the foregroundStyle(by:) modifier to the rectangle mark and passing it a PlottableValue constructed with value(_:_:) which takes a label and the value to plot, in this case `num`. A scale from values of `num` to color will be automatically generated and used to color the rectangles based on the value.

```
struct MatrixEntry {
    var positive: String
    var negative: String
    var num: Double
}

var data: [MatrixEntry] = [
    MatrixEntry(positive: "+", negative: "+", num: 125),
    MatrixEntry(positive: "+", negative: "-", num: 10),
    MatrixEntry(positive: "-", negative: "-", num: 80),
    MatrixEntry(positive: "-", negative: "+", num: 1)
]

var body: some View {
    Chart(data) {
        RectangleMark(
            x: .value("Positive", $0.positive),
            y: .value("Negative", $0.negative)
        )
        .foregroundStyle(by: .value("Number", $0.num))
    }
}
```

### Annotate a Rectangular Area with Rectangle Marks

You can annotate a specific region in a chart with a rectangle mark by providing the coordinates of one or more rectangles. For example you can annotate point marks with rectangle marks using a shared data source like in the example below:

```
struct Coord {
    var x: Double
    var y: Double
}

var data: [Coord] = [
    Coord(x: 5, y: 5),
    Coord(x: 2.5, y: 2.5),
    Coord(x: 3, y: 3)
]

var body: some View {
    Chart(data) {
        RectangleMark(
            xStart: .value("Rect Start Width", $0.x - 0.25),
            xEnd: .value("Rect End Width", $0.x + 0.25),
            yStart: .value("Rect Start Height", $0.y - 0.25),
            yEnd: .value("Rect End Height", $0.y + 0.25)
        )
        .opacity(0.2)

        PointMark(
            x: .value("X", $0.x),
            y: .value("Y", $0.y)
        )
    }
}
```

## Topics

### Creating a rectangle mark

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>, width: MarkDimension)

Creates a rectangle mark with an y interval encoding and an x encoding.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, height: MarkDimension)

Creates a rectangle mark with an x interval encoding and a y encoding.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates a rectangle mark with x and y interval encodings.

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, width: MarkDimension, height: MarkDimension)

Creates a rectangle that plots values with x and y.

### Initializers

init&lt;X>(x: PlottableValue&lt;X>, yStart: CGFloat?, yEnd: CGFloat?, width: MarkDimension)

Creates a rectangle mark that plots values on x and has a fixed y interval.

init&lt;Y>(xStart: CGFloat?, xEnd: CGFloat?, y: PlottableValue&lt;Y>, height: MarkDimension)

Creates a rectangle mark with a fixed x interval and y encoding.

init(xStart: CGFloat?, xEnd: CGFloat?, yStart: CGFloat?, yEnd: CGFloat?)

Creates a rectangle mark with fixed x and y intervals.

init&lt;Y>(xStart: CGFloat?, xEnd: CGFloat?, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates a rectangle mark with a y interval encoding and a fixed x interval.

init&lt;X>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, yStart: CGFloat?, yEnd: CGFloat?)

Creates a rectangle mark with an x interval encoding and a fixed y interval.

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

struct PointMark

Chart content that represents data using points.

struct RuleMark

Chart content that represents data using a single horizontal or vertical rule.

struct BarMark

Chart content that represents data using bars.

struct SectorMark

A sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

