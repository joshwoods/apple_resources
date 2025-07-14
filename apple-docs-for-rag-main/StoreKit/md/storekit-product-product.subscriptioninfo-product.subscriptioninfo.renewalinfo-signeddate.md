

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  signedDate 

Instance Property

# signedDate

The date that the App Store signed the JWS renewal information.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let signedDate: Date
```

## Discussion

Use the signedDate to verify whether the certificate used to sign the transaction was valid when the App Store signed the transaction.

## See Also

### Verifying subscription renewal information

let deviceVerification: Data

The device verification value to use to verify whether the renewal information belongs to the device.

let deviceVerificationNonce: UUID

The UUID to use to compute the device verification value.

