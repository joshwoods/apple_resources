

- Foundation
-  NSDecimalNumberHandler 

Class

# NSDecimalNumberHandler

A class that adopts the decimal number behaviors protocol.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSDecimalNumberHandler
```

## Overview

This class allows you to set the way an NSDecimalNumber object rounds off and handles errors, without having to create a custom class.

You can use an instance of this class as an argument to any of the NSDecimalNumber methods that end with `...Behavior:`. If you don’t think you need special behavior, you probably don’t need this class—it is likely that NSDecimalNumber’s default behavior will suit your needs.

For more information, see the NSDecimalNumberBehaviors protocol specification.

## Topics

### Creating a Decimal Number Handler

class var `default`: NSDecimalNumberHandler

Returns the default instance of `NSDecimalNumberHandler`.

### Initializing a decimal number handler

init(roundingMode: NSDecimalNumber.RoundingMode, scale: Int16, raiseOnExactness: Bool, raiseOnOverflow: Bool, raiseOnUnderflow: Bool, raiseOnDivideByZero: Bool)

Returns an `NSDecimalNumberHandler` object initialized so it behaves as specified by the method’s arguments.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSDecimalNumberBehaviors
- NSObjectProtocol
- Sendable

## See Also

### Configuring Rounding Behavior

var roundingBehavior: NSDecimalNumberHandler

The rounding behavior used by the receiver.

var roundingIncrement: NSNumber!

The rounding increment used by the receiver.

var roundingMode: NumberFormatter.RoundingMode

The rounding mode used by the receiver.

