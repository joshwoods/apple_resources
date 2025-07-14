

- Swift Charts
- PlottableProjection
-  value(\_:\_:unit:calendar:) 

Type Method

# value(\_:\_:unit:calendar:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func value(
    _ labelKey: LocalizedStringKey,
    _ date: KeyPath,
    unit: Calendar.Component,
    calendar: Calendar? = nil
) -> PlottableProjection
```

Available when `DataValue` conforms to `Plottable` and `DataValue.PrimitivePlottable` is `Date`.

