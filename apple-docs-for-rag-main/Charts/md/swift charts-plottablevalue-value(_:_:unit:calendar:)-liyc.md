

- Swift Charts
- PlottableValue
-  value(\_:\_:unit:calendar:) 

Type Method

# value(\_:\_:unit:calendar:)

Creates a parameter value with label and value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func value(
    _ label: Text,
    _ date: Date,
    unit: Calendar.Component,
    calendar: Calendar? = nil
) -> PlottableValue where Value == Date
```

Available when `Value` conforms to `Plottable`.

## Parameters 

`label`  

The label.

