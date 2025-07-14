

- PassKit (Apple Pay and Wallet)
- PKStoredValuePassProperties
-  isBlocked 

Instance Property

# isBlocked

A Boolean value that indicates the pass issuer disabled a stored-value pass.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOSwatchOS 8.0+

``` source
@objc
dynamic var isBlocked: Bool { get }
```

## Discussion

The pass issuer is responsible for blocking a stored-value pass according to their policy. The service provider can’t process transactions for a blocked pass.

## See Also

### Reading the stored-value pass properties

var balances: [PKStoredValuePassBalance]

The amount available for transactions for a service represented by a stored-value pass.

var expirationDate: Date?

The expiration date of a pass.

var isBlacklisted: Bool

A Boolean value that indicates the pass issuer disabled a stored-value pass.

Deprecated

