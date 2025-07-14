

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  deviceVerification 

Instance Property

# deviceVerification

The device verification value to use to verify whether the renewal information belongs to the device.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let deviceVerification: Data
```

## Discussion

For more information, see deviceVerificationID.

## See Also

### Verifying subscription renewal information

let deviceVerificationNonce: UUID

The UUID to use to compute the device verification value.

let signedDate: Date

The date that the App Store signed the JWS renewal information.

