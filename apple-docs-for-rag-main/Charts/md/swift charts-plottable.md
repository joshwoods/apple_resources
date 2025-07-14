

- Swift Charts
-  Plottable 

Protocol

# Plottable

A type that can serve as data to plot in a chart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol Plottable
```

## Overview

You create PlottableValue items from data that conforms to `Plottable` using a method like value(_:_:). You then use those items as the values in a chart, like for the BarMark chart in the following example:

```
BarMark(
  x: .value("Category", "A")
  y: .value("Value", 100)
)
.foregroundStyle(by: .value("Series", "Series 1"))
```

You can create a custom plottable type by conforming it to this protocol. For example:

```
// Make `SomeValue` conform to `Plottable` and act as a categorical value in Swift Charts.
struct SomeValue: Plottable {
    var primitivePlottable: String { ... }
    init?(primitivePlottable: String) { ... }
}
```

In addition, you can make an enum work as a categorical data value by using `String` as its raw value and conforming the type to Plottable. The string values will be used as localized string keys when the categories are displayed as text in a chart (for example, on an axis).

```
enum Status: String, Plottable {
    case active = "Active"
    case inactive = "Inactive"
}
```

## Topics

### Supporting types

protocol PrimitivePlottableProtocol

A type that represents the primitive plottable types supported by the framework. Don’t use this type directly.

### Associated Types

associatedtype PrimitivePlottable : PrimitivePlottableProtocol

A primitive plottable type.

**Required**

### Initializers

init?(primitivePlottable: Self.PrimitivePlottable)

Creates the plottable value for the underlying type, if any, that corresponds to the primitive plottable value.

**Required** Default implementations provided.

### Instance Properties

var primitivePlottable: Self.PrimitivePlottable

The primitive plottable value that corresponds to the plottable value of the underlying type.

**Required** Default implementations provided.

## Relationships

### Inherited By

- PrimitivePlottableProtocol

## See Also

### Labeled data

struct PlottableValue

Labeled data that you plot in a chart using marks.

