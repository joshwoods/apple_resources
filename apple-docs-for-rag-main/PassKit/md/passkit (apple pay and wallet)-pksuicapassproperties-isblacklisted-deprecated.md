

- PassKit (Apple Pay and Wallet)
- PKSuicaPassProperties
-  isBlacklisted Deprecated

Instance Property

# isBlacklisted

A Boolean value that indicates whether the transit pass issuer disabled the pass.

iOS 10.1–15.0DeprecatediPadOS 10.1–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOSvisionOS 1.0–1.0DeprecatedwatchOS 3.1–8.0Deprecated

``` source
var isBlacklisted: Bool { get }
```

Deprecated

Use `PKStoredValuePassProperties` property blocked instead.

## Discussion

Transit pass issuers are responsible for blacklisting transit passes according to their policies. Blacklisted transit passes are not accepted at transit terminals.

## See Also

### Getting pass status

var isBlocked: Bool

A Boolean value that indicates whether the pass issuer disabled the pass.

Deprecated

var isGreenCarTicketUsed: Bool

A Boolean value that indicates whether the customer has redeemed the Green Car ticket.

var isInShinkansenStation: Bool

A Boolean value that indicates whether the pass has tapped in at a Shinkansen Station and has not tapped out.

var isInStation: Bool

A Boolean value that indicates whether the transit pass has tapped in at a station and has not tapped out.

