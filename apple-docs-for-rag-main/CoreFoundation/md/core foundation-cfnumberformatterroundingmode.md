

- Core Foundation
-  CFNumberFormatterRoundingMode 

Enumeration

# CFNumberFormatterRoundingMode

These constants are used to specify how numbers should be rounded.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFNumberFormatterRoundingMode
```

## Topics

### Constants

case roundCeiling

Round towards positive infinity.

case roundFloor

Round towards negative infinity.

case roundDown

Round towards zero.

case roundUp

Round away from zero.

case roundHalfEven

Round towards the nearest integer, or towards an even number if equidistant.

case roundHalfDown

Round towards the nearest integer, or towards zero if equidistant.

case roundHalfUp

Round towards the nearest integer, or away from zero if equidistant.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Number Formatter Styles

Predefined number format styles.

Number Formatter Property Keys

The keys used in key-value pairs to specify the value of number formatter properties.

Number Format Options

These constants are used to specify how numbers should be parsed.

Padding Positions

These constants are used to specify how numbers should be padded.

