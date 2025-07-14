

- Foundation
- NumberFormatter
-  NumberFormatter.Behavior 

Enumeration

# NumberFormatter.Behavior

These constants specify the behavior of a number formatter. These constants are returned by the defaultFormatterBehavior() class method and the formatterBehavior property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Behavior
```

## Topics

### Constants

case `default`

The number-formatter behavior set as the default for new instances. You can set the default formatter behavior with the class method setDefaultFormatterBehavior(_:).

case behavior10_0

The number-formatter behavior as it existed prior to macOS 10.4.

case behavior10_4

The number-formatter behavior since macOS 10.4.

case `default`

The number-formatter behavior set as the default for new instances. You can set the default formatter behavior with the class method setDefaultFormatterBehavior(_:).

case behavior10_0

The number-formatter behavior as it existed prior to macOS 10.4.

case behavior10_4

The number-formatter behavior since macOS 10.4.

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

enum PadPosition

These constants are used to specify how numbers should be padded. These constants are used by the paddingPosition property.

enum RoundingMode

These constants are used to specify how numbers should be rounded. These constants are used by the roundingMode property.

