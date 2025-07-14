

- StoreKit
- Transaction
-  revocationDate 

Instance Property

# revocationDate

The date that the App Store refunded the transaction or revoked it from Family Sharing.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let revocationDate: Date?
```

## Mentioned in 

Testing Family Sharing

Testing refund requests

## See Also

### Getting revocation status

let revocationReason: Transaction.RevocationReason?

The reason that the App Store refunded the transaction or revoked it from Family Sharing.

struct RevocationReason

Reasons that describe why the App Store may refund a transaction or revoke it from Family Sharing.

