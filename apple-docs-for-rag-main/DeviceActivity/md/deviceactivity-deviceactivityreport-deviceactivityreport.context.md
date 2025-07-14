

- DeviceActivity
- DeviceActivityReport
-  DeviceActivityReport.Context 

Structure

# DeviceActivityReport.Context

A context indicating how your device activity report extension should configure its `DeviceActivityReportView`.

DeviceActivitySwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct Context
```

## Overview

You can use a DeviceActivityReport.Context to create a DeviceActivityReport, which the system then provides to your app’s extension and allows it to configure the resulting report `View` in a particular way. For example, if you want to render either a pie chart or bar graph representing the user’s device activity, you can create the following custom contexts:

```
extension DeviceActivityReport.Context {
    static let barGraph = Self("barGraph")
    static let pieChart = Self("pieChart")
}
```

If your app instantiates a report with the `barGraph` context, then the system prompts your report extension to generate a view using the `Scene` corresponding to that context.

## Topics

### Initializers

init(String)

Creates a new instance with the specified raw value.

init(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

The underlying value that represents the given context.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

