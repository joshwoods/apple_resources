

- Swift Charts
- PlottableValue
-  value(\_:\_:) 

Type Method

# value(\_:\_:)

Creates a parameter value with label and value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func value(
    _ label: S,
    _ range: Range
) -> PlottableValue where Value : Comparable, S : StringProtocol
```

Available when `Value` conforms to `Plottable`.

## Parameters 

`label`  

The label.

