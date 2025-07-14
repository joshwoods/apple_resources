

- Accessibility
- AXNumericDataAxisDescriptor
-  valueDescriptionProvider 

Instance Property

# valueDescriptionProvider

A description to speak for a particular data value on the axis.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var valueDescriptionProvider: (Double) -> String { get set }
```

## Mentioned in 

Representing chart data as an audio graph

## Discussion

Use this property to format data values into string representations that include units, dates, times, and more.

