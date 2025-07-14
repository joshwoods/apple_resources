

- Accessibility
- AXNumericDataAxisDescriptor
-  AXNumericDataAxisDescriptor.ScaleType 

Enumeration

# AXNumericDataAxisDescriptor.ScaleType

Constants that describe the scale of a numeric axis.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum ScaleType
```

## Topics

### Scales

case linear

A linear scale.

case ln

A natural log scale.

case log10

A log scale.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the axis scale

var scaleType: AXNumericDataAxisDescriptor.ScaleType

The scale for the axis.

