

- PassKit (Apple Pay and Wallet)
- PKTransitPassProperties
-  isBlacklisted Deprecated

Instance Property

# isBlacklisted

A Boolean value that indicates the transit pass issuer disabled the pass.

iOS 11.3–15.0DeprecatediPadOS 11.3–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 11.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 4.3–8.0Deprecated

``` source
var isBlacklisted: Bool { get }
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

var isBlocked: Bool

A Boolean value that indicates the pass issuer disabled the pass.

Deprecated

