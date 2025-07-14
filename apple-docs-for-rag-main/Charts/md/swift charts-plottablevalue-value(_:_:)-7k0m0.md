

- Swift Charts
- PlottableValue
-  value(\_:\_:) 

Type Method

# value(\_:\_:)

Creates a parameter value with label key and value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func value(
    _ labelKey: LocalizedStringKey,
    _ range: ChartBinRange
) -> PlottableValue where Value : Comparable
```

Available when `Value` conforms to `Plottable`.

## Parameters 

`labelKey`  

The localized string key for label.

`range`  

The parameter’s value.

