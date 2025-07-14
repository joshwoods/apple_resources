

- Swift Charts
-  Chart 

Structure

# Chart

A SwiftUI view that displays a chart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct Chart where Content : ChartContent
```

## Mentioned in 

Creating a chart using Swift Charts

## Overview

To create a chart, instantiate a `Chart` structure with marks that display the properties of your data. For example, suppose you have an array of `ValuePerCategory` structures that define data points composed of a `category` and a `value`:

```
struct ValuePerCategory {
    var category: String
    var value: Double
}

let data: [ValuePerCategory] = [
    .init(category: "A", value: 5),
    .init(category: "B", value: 9),
    .init(category: "C", value: 7)
]
```

You can use BarMark inside a chart to represent the `category` property as different bars in the chart and the `value` property as the y value for each bar:

```
Chart(data, id: \.category) { item in
    BarMark(
        x: .value("Category", item.category),
        y: .value("Value", item.value)
    )
}
```

This chart initializer behaves a lot like a SwiftUI ForEach, creating a mark — in this case, a bar — for each of the values in the `data` array:

### Controlling data series inside a chart

You can compose more sophisticated charts by providing more than one series of marks to the chart. For example, suppose you have profit data for two companies:

```
struct ProfitOverTime {
    var date: Date
    var profit: Double
}

let departmentAProfit: [ProfitOverTime] = 
let departmentBProfit: [ProfitOverTime] = 
```

The following chart creates two different series of LineMark instances with different colors to represent the data for each company. In effect, it moves the `ForEach` construct from the chart’s initializer into the body of the chart, enabling you to represent multiple different series:

```
Chart {
    ForEach(departmentAProfit, id: \.date) { item in
        LineMark(
            x: .value("Date", item.date),
            y: .value("Profit A", item.profit),
            series: .value("Company", "A")
        )
        .foregroundStyle(.blue)
    }
    ForEach(departmentBProfit, id: \.date) { item in
        LineMark(
            x: .value("Date", item.date),
            y: .value("Profit B", item.profit),
            series: .value("Company", "B")
        )
        .foregroundStyle(.green)
    }
    RuleMark(
        y: .value("Threshold", 400)
    )
    .foregroundStyle(.red)
}
```

You indicate which series a line mark belongs to by specifying its `series` input parameter. The above chart also uses a RuleMark to produce a horizontal line segment that displays a constant threshold value across the width of the chart:

## Topics

### Creating a chart

init(content: () -> Content)

Creates a chart composed of any number of data series and individual marks.

init&lt;Data, C>(Data, content: (Data.Element) -> C)

Creates a chart composed of a series of identifiable marks.

init&lt;Data, ID, C>(Data, id: KeyPath&lt;Data.Element, ID>, content: (Data.Element) -> C)

Creates a chart composed of a series of marks.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Charts

Creating a chart using Swift Charts

Make a chart by combining chart building blocks in SwiftUI.

Visualizing your app’s data

Build complex and interactive charts using Swift Charts.

protocol ChartContent

A type that represents the content that you draw on a chart.

struct ChartContentBuilder

A result builder that you use to compose the contents of a chart.

struct Plot

A mechanism for grouping chart contents into a single entity.

