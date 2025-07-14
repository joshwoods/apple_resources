

- PassKit (Apple Pay and Wallet)
- PKStoredValuePassProperties
-  balances 

Instance Property

# balances

The amount available for transactions for a service represented by a stored-value pass.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSvisionOS 1.0+watchOS 8.0+

``` source
var balances: [PKStoredValuePassBalance] { get }
```

## See Also

### Reading the stored-value pass properties

var expirationDate: Date?

The expiration date of a pass.

var isBlocked: Bool

A Boolean value that indicates the pass issuer disabled a stored-value pass.

var isBlacklisted: Bool

A Boolean value that indicates the pass issuer disabled a stored-value pass.

Deprecated

