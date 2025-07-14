

- Foundation
- NSDecimalNumber
-  dividing(by:) 

Instance Method

# dividing(by:)

Divides the number by another given number.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dividing(by decimalNumber: NSDecimalNumber) -> NSDecimalNumber
```

## Parameters 

`decimalNumber`  

The number by which to divide the receiver.

## Return Value

A new `NSDecimalNumber` object whose value is the value of the receiver divided by `decimalNumber`.

## Discussion

This method uses the default behavior when handling calculation errors and rounding.

## See Also

### Related Documentation

class var defaultBehavior: any NSDecimalNumberBehaviors

The way arithmetic methods round off and handle error conditions.

### Performing Arithmetic

func adding(NSDecimalNumber) -> NSDecimalNumber

Adds this number to another given number.

func subtracting(NSDecimalNumber) -> NSDecimalNumber

Subtracts another given number from this one.

func multiplying(by: NSDecimalNumber) -> NSDecimalNumber

Multiplies the number by another given number.

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

