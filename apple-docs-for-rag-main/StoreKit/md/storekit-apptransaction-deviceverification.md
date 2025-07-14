

- StoreKit
- AppTransaction
-  deviceVerification 

Instance Property

# deviceVerification

The device verification value to use to verify whether the app transaction belongs to the device.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let deviceVerification: Data
```

## Discussion

For more information, see deviceVerificationID.

## See Also

### Verifying the app transaction

let deviceVerificationNonce: UUID

The UUID used to compute the device verification value.

let signedDate: Date

The date that the App Store signed the JWS app transaction.

