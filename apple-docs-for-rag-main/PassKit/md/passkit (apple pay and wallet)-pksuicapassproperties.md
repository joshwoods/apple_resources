

- PassKit (Apple Pay and Wallet)
-  PKSuicaPassProperties 

Class

# PKSuicaPassProperties

The properties of a pass used as a ticket for the Suica transportation system.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 3.1+

``` source
class PKSuicaPassProperties
```

## Overview

The Suica pass is a card used for transportation in Japan.

## Topics

### Initializing suica pass properties

convenience init?(for: PKPass)

Instantiates a Suica pass properties object that contains the properties supported in the specified pass.

### Getting pass status

var isBlocked: Bool

A Boolean value that indicates whether the pass issuer disabled the pass.

Deprecated

var isBlacklisted: Bool

A Boolean value that indicates whether the transit pass issuer disabled the pass.

Deprecated

var isGreenCarTicketUsed: Bool

A Boolean value that indicates whether the customer has redeemed the Green Car ticket.

var isInShinkansenStation: Bool

A Boolean value that indicates whether the pass has tapped in at a Shinkansen Station and has not tapped out.

var isInStation: Bool

A Boolean value that indicates whether the transit pass has tapped in at a station and has not tapped out.

### Getting suica balance information

var transitBalance: NSDecimalNumber

The current usable stored value on the transit card.

var transitBalanceCurrencyCode: String

The currency code associated with the balance on the pass.

var isBalanceAllowedForCommute: Bool

A Boolean value that indicates how the balance can be used.

var isLowBalanceGateNotificationEnabled: Bool

A Boolean value that determines whether the terminal provides feedback if the balance is low after a deduction.

## Relationships

### Inherits From

- PKTransitPassProperties

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

class PKStoredValuePassProperties

An object that represents the properties of a pass that contains a balance used for specific transactions, such as a transit pass or loyalty card.

class PKStoredValuePassBalance

An object that represents a balance that’s available for transactions, such as points or money.

