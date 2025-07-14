

- PassKit (Apple Pay and Wallet)
- PKTransitPassProperties
-  isBlocked Deprecated

Instance Property

# isBlocked

A Boolean value that indicates the pass issuer disabled the pass.

iOS 14.5+iPadOS 14.5+Mac CatalystmacOS 11.3+visionOSwatchOS 7.5+

``` source
override dynamic var isBlocked: Bool { get }
```

Deprecated

Use `PKStoredValuePassProperties` property blocked instead.

## Discussion

A blocked pass isn’t accepted at a transit terminal.

## See Also

### Getting pass status

var expirationDate: Date?

The date that the transit card expires.

var isInStation: Bool

A Boolean value that indicates whether the transit pass has tapped in at a station and has not tapped out.

var isBlacklisted: Bool

A Boolean value that indicates the transit pass issuer disabled the pass.

Deprecated

