

- PassKit (Apple Pay and Wallet)
- PKStoredValuePassProperties
-  isBlacklisted Deprecated

Instance Property

# isBlacklisted

A Boolean value that indicates the pass issuer disabled a stored-value pass.

iOS 15.0–15.0DeprecatediPadOS 15.0–15.0DeprecatedMac Catalyst 15.0–15.0DeprecatedmacOS 12.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 8.0–8.0Deprecated

``` source
var isBlacklisted: Bool { get }
```

Deprecated

Use `PKStoredValuePassProperties` property blocked instead.

## See Also

### Reading the stored-value pass properties

var balances: [PKStoredValuePassBalance]

The amount available for transactions for a service represented by a stored-value pass.

var expirationDate: Date?

The expiration date of a pass.

var isBlocked: Bool

A Boolean value that indicates the pass issuer disabled a stored-value pass.

