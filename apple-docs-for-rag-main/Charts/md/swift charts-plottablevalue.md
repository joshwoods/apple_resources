

- Swift Charts
-  PlottableValue 

Structure

# PlottableValue

Labeled data that you plot in a chart using marks.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct PlottableValue where Value : Plottable
```

## Overview

Provide a `PlottableValue` to a `Mark` property (e.g., x, y, foregroundStyle) to plot data values with the mark property.

Important

The data type must conform to Plottable. This is a numeric value like a Double or Int16 for quantitative data, Date for temporal data, or String for categorical data.

You can use the `.value("Category", \.category)` shorthand to create a `PlottableValue`. The example below plots category, value, and group with the bar mark’s x, y, and foregroundStyle.

```
struct Bar {
    let category: String
    let value: Double
    let group: String
}

let data: [Bar] = [
    Bar(category: "A", value: 20, group: "Group 1"),
    Bar(category: "A", value: 30, group: "Group 2"),
    Bar(category: "A", value: 10, group: "Group 3"),
    Bar(category: "B", value: 40, group: "Group 1"),
    Bar(category: "B", value: 20, group: "Group 2"),
    Bar(category: "B", value: 10, group: "Group 3"),
    //...
]

var body: some View {
    Chart(data) {
        BarMark(
            x: .value("Category", $0.category),
            y: .value("Quantity", $0.value)
        )
        .foregroundStyle(.value("Group", $0.group))
    }
}
```

## Topics

### Type Methods

static func value&lt;S>(S, Value) -> PlottableValue&lt;Value>

Creates a parameter value with label and value.

static func value(LocalizedStringKey, Range&lt;Value>) -> PlottableValue&lt;Value>

Creates a parameter value with label key and value.

static func value(Text, Range&lt;Value>) -> PlottableValue&lt;Value>

Creates a parameter value with label and value.

static func value&lt;S>(S, ChartBinRange&lt;Value>) -> PlottableValue&lt;Value>

Creates a parameter value with label and value.

static func value(LocalizedStringKey, Value) -> PlottableValue&lt;Value>

Creates a parameter value with label key and value.

static func value(Text, Value) -> PlottableValue&lt;Value>

Creates a parameter value with label and value.

static func value(LocalizedStringKey, ChartBinRange&lt;Value>) -> PlottableValue&lt;Value>

Creates a parameter value with label key and value.

static func value(Text, ChartBinRange&lt;Value>) -> PlottableValue&lt;Value>

Creates a parameter value with label and value.

static func value&lt;S>(S, Range&lt;Value>) -> PlottableValue&lt;Value>

Creates a parameter value with label and value.

static func value&lt;S>(S, Date, unit: Calendar.Component, calendar: Calendar?) -> PlottableValue&lt;Value>

Creates a parameter value with label and value.

static func value(LocalizedStringKey, Date, unit: Calendar.Component, calendar: Calendar?) -> PlottableValue&lt;Value>

Creates a parameter value with label key and value.

static func value(Text, Date, unit: Calendar.Component, calendar: Calendar?) -> PlottableValue&lt;Value>

Creates a parameter value with label and value.

## See Also

### Labeled data

protocol Plottable

A type that can serve as data to plot in a chart.

