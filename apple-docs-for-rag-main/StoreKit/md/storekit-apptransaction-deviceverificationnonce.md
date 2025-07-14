

- StoreKit
- AppTransaction
-  deviceVerificationNonce 

Instance Property

# deviceVerificationNonce

The UUID used to compute the device verification value.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let deviceVerificationNonce: UUID
```

## Discussion

For more information, see deviceVerificationID.

## See Also

### Verifying the app transaction

let deviceVerification: Data

The device verification value to use to verify whether the app transaction belongs to the device.

let signedDate: Date

The date that the App Store signed the JWS app transaction.

