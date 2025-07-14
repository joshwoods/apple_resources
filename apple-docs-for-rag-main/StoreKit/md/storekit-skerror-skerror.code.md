

- StoreKit
- SKError
-  SKError.Code 

Enumeration

# SKError.Code

Error codes for StoreKit errors.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+watchOS 6.2+

``` source
enum Code
```

## Mentioned in 

Handling errors

## Topics

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

case invalidSignature

Error code indicating that the signature in a payment discount isn’t valid.

case missingOfferParams

Error code indicating that parameters are missing in a payment discount.

case ineligibleForOffer

An error code that indicates the user is ineligible for the subscription offer.

case overlayCancelled

An error code that indicates the cancellation of an overlay.

case overlayInvalidConfiguration

An error code that indicates the overlay’s configuration is invalid.

case overlayPresentedInBackgroundScene

case overlayTimeout

case unsupportedPlatform

An error code that indicates the current platform doesn’t support overlays.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

Handling errors

Determine the underlying cause of errors that result from StoreKit requests.

struct SKError

StoreKit error descriptions, codes, and domains.

let SKErrorDomain: String

The error domain name for StoreKit errors.

