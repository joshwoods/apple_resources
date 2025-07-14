

- PassKit (Apple Pay and Wallet)
- PKSuicaPassProperties
-  isBlocked Deprecated

Instance Property

# isBlocked

A Boolean value that indicates whether the pass issuer disabled the pass.

iOS 10.1+iPadOS 10.1+Mac CatalystmacOSvisionOSwatchOS 3.1+

``` source
override dynamic var isBlocked: Bool { get }
```

Deprecated

Use `PKStoredValuePassProperties` property blocked instead.

## See Also

### Getting pass status

var isBlacklisted: Bool

A Boolean value that indicates whether the transit pass issuer disabled the pass.

Deprecated

var isGreenCarTicketUsed: Bool

A Boolean value that indicates whether the customer has redeemed the Green Car ticket.

var isInShinkansenStation: Bool

A Boolean value that indicates whether the pass has tapped in at a Shinkansen Station and has not tapped out.

var isInStation: Bool

A Boolean value that indicates whether the transit pass has tapped in at a station and has not tapped out.

