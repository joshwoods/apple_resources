

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  deviceVerificationNonce 

Instance Property

# deviceVerificationNonce

The UUID to use to compute the device verification value.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let deviceVerificationNonce: UUID
```

## Discussion

For more information, see deviceVerificationID.

## See Also

### Verifying subscription renewal information

let deviceVerification: Data

The device verification value to use to verify whether the renewal information belongs to the device.

let signedDate: Date

The date that the App Store signed the JWS renewal information.

