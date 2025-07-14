

- Swift Charts
-  RuleMark 

Structure

# RuleMark

Chart content that represents data using a single horizontal or vertical rule.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct RuleMark
```

## Overview

You can use `RuleMark` to plot a horizontal or vertical rule in your chart.

### Show Range with Rule Marks

To create a horizontal line at a `y` position from `xStart` to `xEnd` you use the `init(xStart:xEnd:y:)` or `init(xStart:xEnd:y:)`. To create a vertical line at an `x` position from `yStart` to `yEnd` you use `init(x:yStart:yEnd:)` or `init(x:yStart:yEnd:)`. The example below uses the `Pollen` structure and the `init(xStart:xEnd:y:)` to map horizontal lines that span from the value of the `startDate` to the value of the `endDate` for x positions to a pollen `source` property’s y position:

```
struct Pollen {
    var source: String
    var startDate: Date
    var endDate: Date

    init(startMonth: Int, numMonths: Int, source: String) {
        self.source = source
        let calendar = Calendar.autoupdatingCurrent
        self.startDate = calendar.date(from: DateComponents(year: 2020, month: startMonth, day: 1))!
        self.endDate = calendar.date(byAdding: .month, value: numMonths, to: startDate)!
    }
}

var data: [Pollen] = [
    Pollen(startMonth: 1, numMonths: 9, source: "Trees"),
    Pollen(startMonth: 12, numMonths: 1, source: "Trees"),
    Pollen(startMonth: 3, numMonths: 8, source: "Grass"),
    Pollen(startMonth: 4, numMonths: 8, source: "Weeds")
]

var body: some View {
    Chart(data) {
        RuleMark(
            xStart: .value("Start Date", $0.startDate),
            xEnd: .value("End Date", $0.endDate),
            y: .value("Pollen Source", $0.source)
        )
    }
}
```

### Annotate a chart with rule mark

You can annotate a chart with horizontal or vertically spanning rules. This allows viewers to easily compare values over a range to a constant value. Use theinit(xStart:xEnd:y:) initializer to represent a constant `y` value or init(x:yStart:yEnd:) for a constant `x` value. To span the plotting area of a chart with a line, omit the optional start and end parameters and plot a constant value. The example below results in a line that spans the chart horizontally at the y position of 9000:

```
struct DepartmentProfit {
    var department: String
    var profit: Double
}

var data: [DepartmentProfit] = [
    DepartmentProfit(department: "Production", profit: 15000),
    DepartmentProfit(department: "Marketing", profit: 8000),
    DepartmentProfit(department: "Finance", profit: 10000)
]

var body: some View {
    Chart
        ForEach(data) {
            BarMark(
                x: .value("Department", $0.department),
                y: .value("Profit", $0.profit)
            )
        }
        RuleMark(y: .value("Break Even Threshold", 9000))
            .foregroundStyle(.red)
    }
}
```

## Topics

### Initializers

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates a vertical rule mark with an x encoding and y interval encoding.

init&lt;X>(x: PlottableValue&lt;X>, yStart: CGFloat?, yEnd: CGFloat?)

Creates a vertical rule mark with value plotted with x.

init&lt;Y>(x: CGFloat?, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates a vertical rule mark with a fixed x position and y interval encoding.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>)

Creates a horizontal rule mark that plots values on its x interval and on y.

init&lt;Y>(xStart: CGFloat?, xEnd: CGFloat?, y: PlottableValue&lt;Y>)

Creates a horizontal rule mark that plots a value on y.

init&lt;X>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: CGFloat?)

Creates a horizontal rule mark that plots values on its x interval.

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

struct RectangleMark

Chart content that represents data using rectangles.

struct BarMark

Chart content that represents data using bars.

struct SectorMark

A sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

