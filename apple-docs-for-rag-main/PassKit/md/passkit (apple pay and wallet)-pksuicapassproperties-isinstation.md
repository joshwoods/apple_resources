

- PassKit (Apple Pay and Wallet)
- PKSuicaPassProperties
-  isInStation 

Instance Property

# isInStation

A Boolean value that indicates whether the transit pass has tapped in at a station and has not tapped out.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 3.1+

``` source
var isInStation: Bool { get }
```

## Discussion

Transit networks that have tap-in and tap-out ride accounting use this value. Wallet may display this status as “en-route” in its user interface.

## See Also

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

