

- StoreKit
- AppTransaction
-  signedDate 

Instance Property

# signedDate

The date that the App Store signed the JWS app transaction.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let signedDate: Date
```

## Discussion

Use the signedDate to verify whether the certificate used to sign the app transaction was valid when the App Store signed the transaction.

## See Also

### Verifying the app transaction

let deviceVerification: Data

The device verification value to use to verify whether the app transaction belongs to the device.

let deviceVerificationNonce: UUID

The UUID used to compute the device verification value.

