

- PassKit (Apple Pay and Wallet)
- PKTransitPassProperties
-  expirationDate 

Instance Property

# expirationDate

The date that the transit card expires.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.3+

``` source
var expirationDate: Date? { get }
```

## Discussion

Rules for expiry depend on the pass provider. The return value can be `nil` if the transit card does not support an expiration date.

## See Also

### Getting pass status

var isInStation: Bool

A Boolean value that indicates whether the transit pass has tapped in at a station and has not tapped out.

var isBlocked: Bool

A Boolean value that indicates the pass issuer disabled the pass.

Deprecated

var isBlacklisted: Bool

A Boolean value that indicates the transit pass issuer disabled the pass.

Deprecated

