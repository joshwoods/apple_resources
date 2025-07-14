

- StoreKit
- Transaction
-  signedDate 

Instance Property

# signedDate

The date that the App Store signed the JWS transaction.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let signedDate: Date
```

## Discussion

Use the signedDate to verify whether the certificate used to sign the transaction was valid when the App Store signed the transaction.

## See Also

### Verifying transactions

let deviceVerification: Data

The device verification value you use to verify whether the transaction belongs to the device.

let deviceVerificationNonce: UUID

The UUID for computing the device verification value.

