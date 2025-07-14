

- PassKit (Apple Pay and Wallet)
- PKTransitPassProperties
-  isInStation 

Instance Property

# isInStation

A Boolean value that indicates whether the transit pass has tapped in at a station and has not tapped out.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 4.3+

``` source
var isInStation: Bool { get }
```

## Discussion

Transit networks that have tap-in and tap-out ride accounting use this value. Wallet may display this status as “en-route” in its user interface.

## See Also

### Getting pass status

var expirationDate: Date?

The date that the transit card expires.

var isBlocked: Bool

A Boolean value that indicates the pass issuer disabled the pass.

Deprecated

var isBlacklisted: Bool

A Boolean value that indicates the transit pass issuer disabled the pass.

Deprecated

