

- PassKit (Apple Pay and Wallet)
-  PKTransitPassProperties 

Class

# PKTransitPassProperties

The properties of a transit pass.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 4.3+

``` source
class PKTransitPassProperties
```

## Topics

### Getting pass status

var expirationDate: Date?

The date that the transit card expires.

var isInStation: Bool

A Boolean value that indicates whether the transit pass has tapped in at a station and has not tapped out.

var isBlocked: Bool

A Boolean value that indicates the pass issuer disabled the pass.

Deprecated

var isBlacklisted: Bool

A Boolean value that indicates the transit pass issuer disabled the pass.

Deprecated

### Getting balance information

var transitBalance: NSDecimalNumber

The current usable stored value on the transit card.

Deprecated

var transitBalanceCurrencyCode: String

The currency code associated with the balance on the pass.

Deprecated

## Relationships

### Inherits From

- PKStoredValuePassProperties

### Inherited By

- PKSuicaPassProperties

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Stored-value passes

class PKSuicaPassProperties

The properties of a pass used as a ticket for the Suica transportation system.

class PKStoredValuePassProperties

An object that represents the properties of a pass that contains a balance used for specific transactions, such as a transit pass or loyalty card.

class PKStoredValuePassBalance

An object that represents a balance that’s available for transactions, such as points or money.

