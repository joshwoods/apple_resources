

- Foundation
- NumberFormatter
-  NumberFormatter.RoundingMode 

Enumeration

# NumberFormatter.RoundingMode

These constants are used to specify how numbers should be rounded. These constants are used by the roundingMode property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum RoundingMode
```

## Topics

### Constants

case ceiling

Round towards positive infinity.

case floor

Round towards negative infinity.

case down

Round towards zero.

case up

Round away from zero.

case halfEven

Round towards the nearest integer, or towards an even number if equidistant.

case halfDown

Round towards the nearest integer, or towards zero if equidistant.

case halfUp

Round towards the nearest integer, or away from zero if equidistant.

case ceiling

Round towards positive infinity.

case floor

Round towards negative infinity.

case down

Round towards zero.

case up

Round away from zero.

case halfEven

Round towards the nearest integer, or towards an even number if equidistant.

case halfDown

Round towards the nearest integer, or towards zero if equidistant.

case halfUp

Round towards the nearest integer, or away from zero if equidistant.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum Style

The predefined number format styles used by the numberStyle property.

enum Behavior

These constants specify the behavior of a number formatter. These constants are returned by the defaultFormatterBehavior() class method and the formatterBehavior property.

enum PadPosition

These constants are used to specify how numbers should be padded. These constants are used by the paddingPosition property.

