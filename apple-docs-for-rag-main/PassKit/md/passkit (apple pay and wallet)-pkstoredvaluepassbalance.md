

- PassKit (Apple Pay and Wallet)
-  PKStoredValuePassBalance 

Class

# PKStoredValuePassBalance

An object that represents a balance that’s available for transactions, such as points or money.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSvisionOS 1.0+watchOS 8.0+

``` source
class PKStoredValuePassBalance
```

## Overview

Important

A stored balance of type of cash requires a valid currency code.

## Topics

### Getting the pass status

var expiryDate: Date?

The date that the balance expires.

var amount: Decimal

The current balance of a stored-value pass in money or points.

var balanceType: PKStoredValuePassBalance.BalanceType

The type of value that the balance represents, such as money or points.

var currencyCode: String?

The ISO 4217 currency code of the balance.

struct BalanceType

The type of value that the balance represents, such as money or points.

### Comparing pass balance objects

static func == (PKStoredValuePassBalance, PKStoredValuePassBalance) -> Bool

Returns a Boolean value that indicates whether two pass balance objects contain the same values.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Stored-value passes

class PKTransitPassProperties

The properties of a transit pass.

class PKSuicaPassProperties

The properties of a pass used as a ticket for the Suica transportation system.

class PKStoredValuePassProperties

An object that represents the properties of a pass that contains a balance used for specific transactions, such as a transit pass or loyalty card.

