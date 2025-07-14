

- Swift Charts
- PlottableProjection
-  value(\_:\_:\_:) 

Type Method

# value(\_:\_:\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func value(
    _ labelKey: LocalizedStringKey,
    _ start: KeyPath,
    _ end: KeyPath
) -> PlottableProjection where DataValue : Comparable
```

Available when `DataValue` conforms to `Plottable`.

