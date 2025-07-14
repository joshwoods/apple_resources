

- Metal Performance Shaders Graph
-  MPSGraphResizeNearestRoundingMode 

Enumeration

# MPSGraphResizeNearestRoundingMode

The rounding mode to use when using nearest resize mode.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MPSGraphResizeNearestRoundingMode
```

## Topics

### Enumeration Cases

case ceil

Rounds values toward +inf.

case floor

Rounds values toward -inf.

case roundPreferCeil

Rounds values to the nearest integer value, with 0.5f offset rounding toward +inf.

case roundPreferFloor

Rounds values to the nearest integer value, with 0.5f rounding toward -inf.

case roundToEven

Rounds values to the nearest integer value, with 0.5f rounding toward the closest even value.

case roundToOdd

Rounds values to the nearest integer value, with 0.5f rounding toward the closest odd value.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

