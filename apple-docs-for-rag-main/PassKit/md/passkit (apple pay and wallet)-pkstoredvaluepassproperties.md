

- PassKit (Apple Pay and Wallet)
-  PKStoredValuePassProperties 

Class

# PKStoredValuePassProperties

An object that represents the properties of a pass that contains a balance used for specific transactions, such as a transit pass or loyalty card.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSvisionOS 1.0+watchOS 8.0+

``` source
class PKStoredValuePassProperties
```

## Topics

### Creating a stored-value pass properties object

convenience init?(for: PKPass)

Creates a stored-value pass properties object for the specified pass.

### Reading the stored-value pass properties

var balances: [PKStoredValuePassBalance]

The amount available for transactions for a service represented by a stored-value pass.

var expirationDate: Date?

The expiration date of a pass.

var isBlocked: Bool

A Boolean value that indicates the pass issuer disabled a stored-value pass.

var isBlacklisted: Bool

A Boolean value that indicates the pass issuer disabled a stored-value pass.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

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

class PKSuicaPassProperties

The properties of a pass used as a ticket for the Suica transportation system.

class PKStoredValuePassBalance

An object that represents a balance that’s available for transactions, such as points or money.

