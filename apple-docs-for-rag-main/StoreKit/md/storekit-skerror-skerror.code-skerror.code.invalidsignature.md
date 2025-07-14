

- StoreKit
- SKError
- SKError.Code
-  SKError.Code.invalidSignature 

Case

# SKError.Code.invalidSignature

Error code indicating that the signature in a payment discount isn’t valid.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+macOS 10.14.4+tvOS 12.2+visionOS 1.0+watchOS 6.2+

``` source
case invalidSignature
```

## Discussion

The signature is not valid.

## See Also

### Enumeration Cases

case unknown

Error code indicating that an unknown or unexpected error occurred.

case clientInvalid

Error code indicating that the client is not allowed to perform the attempted action.

case paymentCancelled

Error code indicating that the user canceled a payment request.

case paymentInvalid

Error code indicating that one of the payment parameters wasn’t recognized by the App Store.

case paymentNotAllowed

Error code indicating that the user is not allowed to authorize payments.

case storeProductNotAvailable

Error code indicating that the requested product is not available in the store.

case cloudServicePermissionDenied

Error code indicating that the user has not allowed access to Cloud service information.

case cloudServiceNetworkConnectionFailed

Error code indicating that the device could not connect to the network.

case cloudServiceRevoked

Error code indicating that the user has revoked permission to use this cloud service.

case privacyAcknowledgementRequired

Error code indicating that the user has not yet acknowledged Apple’s privacy policy for Apple Music.

case unauthorizedRequestData

Error code indicating that the app is attempting to use a property for which it does not have the required entitlement.

case invalidOfferIdentifier

Error code indicating that the offer identifier is invalid.

case invalidOfferPrice

Error code indicating that the price you specified in App Store Connect is no longer valid.

case missingOfferParams

Error code indicating that parameters are missing in a payment discount.

case ineligibleForOffer

An error code that indicates the user is ineligible for the subscription offer.

