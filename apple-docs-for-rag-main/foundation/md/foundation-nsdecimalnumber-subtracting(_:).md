

- Foundation
- NSDecimalNumber
-  subtracting(\_:) 

Instance Method

# subtracting(\_:)

Subtracts another given number from this one.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func subtracting(_ decimalNumber: NSDecimalNumber) -> NSDecimalNumber
```

## Parameters 

`decimalNumber`  

The number to subtract from the receiver.

## Return Value

A new `NSDecimalNumber` object whose value is `decimalNumber` subtracted from the receiver.

## Discussion

This method uses the default behavior when handling calculation errors and when rounding.

## See Also

### Related Documentation

class var defaultBehavior: any NSDecimalNumberBehaviors

The way arithmetic methods round off and handle error conditions.

### Performing Arithmetic

func adding(NSDecimalNumber) -> NSDecimalNumber

Adds this number to another given number.

func multiplying(by: NSDecimalNumber) -> NSDecimalNumber

Multiplies the number by another given number.

func dividing(by: NSDecimalNumber) -> NSDecimalNumber

Divides the number by another given number.

func raising(toPower: Int) -> NSDecimalNumber

Raises the number to a given power.

func multiplying(byPowerOf10: Int16) -> NSDecimalNumber

Multiplies the number by 10 raised to the given power.

func adding(NSDecimalNumber, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Adds this number to another given number using the specified behavior.

func subtracting(NSDecimalNumber, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Subtracts this a given number from this one using the specified behavior.

func multiplying(by: NSDecimalNumber, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Multiplies this number by another given number using the specified behavior.

func dividing(by: NSDecimalNumber, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Divides this number by another given number using the specified behavior.

func raising(toPower: Int, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Raises the number to a given power using the specified behavior.

func multiplying(byPowerOf10: Int16, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Multiplies the number by 10 raised to the given power using the specified behavior.

