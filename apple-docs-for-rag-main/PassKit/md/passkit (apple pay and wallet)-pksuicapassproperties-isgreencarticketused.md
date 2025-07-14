

- PassKit (Apple Pay and Wallet)
- PKSuicaPassProperties
-  isGreenCarTicketUsed 

Instance Property

# isGreenCarTicketUsed

A Boolean value that indicates whether the customer has redeemed the Green Car ticket.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 3.1+

``` source
var isGreenCarTicketUsed: Bool { get }
```

## Discussion

A Green Car ticket is valid for a single use. This flag indicates the ticket has been used and is not eligible for a refund.

## See Also

### Getting pass status

var isBlocked: Bool

A Boolean value that indicates whether the pass issuer disabled the pass.

Deprecated

var isBlacklisted: Bool

A Boolean value that indicates whether the transit pass issuer disabled the pass.

Deprecated

var isInShinkansenStation: Bool

A Boolean value that indicates whether the pass has tapped in at a Shinkansen Station and has not tapped out.

var isInStation: Bool

A Boolean value that indicates whether the transit pass has tapped in at a station and has not tapped out.

