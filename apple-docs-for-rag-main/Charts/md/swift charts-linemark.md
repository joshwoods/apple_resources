

- Swift Charts
-  LineMark 

Structure

# LineMark

Chart content that represents data using a sequence of connected line segments.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct LineMark
```

## Mentioned in 

Creating a chart using Swift Charts

## Overview

You create a line chart by plotting a category or date property, typically with the x position, and plotting a number category, typically with the y position. The example below plots the `date` property to the x position and the `hoursOfSunshine` property to the y position using init(x:y:):

```
struct MonthlyHoursOfSunshine {
    var date: Date
    var hoursOfSunshine: Double

    init(month: Int, hoursOfSunshine: Double) {
        let calendar = Calendar.autoupdatingCurrent
        self.date = calendar.date(from: DateComponents(year: 2020, month: month))!
        self.hoursOfSunshine = hoursOfSunshine
    }
}

var data: [MonthlyHoursOfSunshine] = [
    MonthlyHoursOfSunshine(month: 1, hoursOfSunshine: 74),
    MonthlyHoursOfSunshine(month: 2, hoursOfSunshine: 99),
    // ...
    MonthlyHoursOfSunshine(month: 12, hoursOfSunshine: 62)
]

var body: some View {
    Chart(data) {
        LineMark(
            x: .value("Month", $0.date),
            y: .value("Hours of Sunshine", $0.hoursOfSunshine)
        )
    }
}
```

### Plotting multiple lines

You can plot multiple lines in a chart either by explicitly specifying the `series` parameter in init(x:y:series:) or by applying the foregroundStyle(_:) or lineStyle(_:) modifiers. Line marks with the same `series` value will always be rendered together as a single line. When `series` is unspecified line marks with the same value plotted to foreground style and line style will be grouped together and plotted on their own line. The example below plots one line per distinct value in `city` and colors each line based on the `city` it represents:

```
struct MonthlyHoursOfSunshine {
    var city: String
    var date: Date
    var hoursOfSunshine: Double

    init(city: String, month: Int, hoursOfSunshine: Double) {
        let calendar = Calendar.autoupdatingCurrent
        self.city = city
        self.date = calendar.date(from: DateComponents(year: 2020, month: month))!
        self.hoursOfSunshine = hoursOfSunshine
    }
}

var data: [MonthlyHoursOfSunshine] = [
    MonthlyHoursOfSunshine(city: "Seattle", month: 1, hoursOfSunshine: 74),
    MonthlyHoursOfSunshine(city: "Cupertino", month: 1, hoursOfSunshine: 196),
    // ...
    MonthlyHoursOfSunshine(city: "Seattle", month: 12, hoursOfSunshine: 62),
    MonthlyHoursOfSunshine(city: "Cupertino", month: 12, hoursOfSunshine: 199)
]

var body: some View {
    Chart(data) {
        LineMark(
            x: .value("Month", $0.date),
            y: .value("Hours of Sunshine", $0.hoursOfSunshine)
        )
        .foregroundStyle(by: .value("City", $0.city))
    }
}
```

Note

Colors are repeated if the number of series is greater than the total number of colors.

## Topics

### Creating a line mark

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>)

Creates a line mark.

init&lt;X, Y, S>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates a separate line for each unique value of series.

## Relationships

### Conforms To

- ChartContent
- Copyable
- Sendable

## See Also

### Marks

struct AreaMark

Chart content that represents data using the area of one or more regions.

struct PointMark

Chart content that represents data using points.

struct RectangleMark

Chart content that represents data using rectangles.

struct RuleMark

Chart content that represents data using a single horizontal or vertical rule.

struct BarMark

Chart content that represents data using bars.

struct SectorMark

A sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

