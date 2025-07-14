

- StoreKit
-  SKError 

Structure

# SKError

StoreKit error descriptions, codes, and domains.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+watchOS 6.2+

``` source
struct SKError
```

## Topics

### Error codes

enum Code

Error codes for StoreKit errors.

static var unknown: SKError.Code

Error code indicating that an unknown or unexpected error occurred.

static var clientInvalid: SKError.Code

Error code indicating that the client is not allowed to perform the attempted action.

static var paymentCancelled: SKError.Code

Error code indicating that the user canceled a payment request.

static var paymentInvalid: SKError.Code

Error code indicating that one of the payment parameters was not recognized by the App Store.

static var paymentNotAllowed: SKError.Code

Error code indicating that the user is not allowed to authorize payments.

static var storeProductNotAvailable: SKError.Code

Error code indicating that the requested product is not available in the store.

static var cloudServicePermissionDenied: SKError.Code

Error code indicating that the user has not allowed access to Cloud service information.

static var cloudServiceNetworkConnectionFailed: SKError.Code

Error code indicating that the device could not connect to the network.

static var cloudServiceRevoked: SKError.Code

Error code indicating that the user has revoked permission to use this cloud service.

static var privacyAcknowledgementRequired: SKError.Code

Error code indicating that the user has not yet acknowledged Apple’s privacy policy for Apple Music.

static var unauthorizedRequestData: SKError.Code

Error code indicating that the app is attempting to use a property for which it does not have the required entitlement.

static var invalidOfferIdentifier: SKError.Code

Error code indicating that the offer identifier cannot be found or is not active.

static var invalidOfferPrice: SKError.Code

Error code indicating that the price you specified in App Store Connect is no longer valid.

static var invalidSignature: SKError.Code

Error code indicating that the signature in a payment discount is not valid.

static var missingOfferParams: SKError.Code

Error code indicating that parameters are missing in a payment discount.

static var ineligibleForOffer: SKError.Code

An error code that indicates the user is ineligible for the subscription offer.

static var overlayCancelled: SKError.Code

An error code that indicates the cancellation of an overlay.

static var overlayInvalidConfiguration: SKError.Code

An error code that indicates the overlay’s configuration is invalid.

static var overlayPresentedInBackgroundScene: SKError.Code

static var overlayTimeout: SKError.Code

An error code that indicates the timing out of an overlay.

static var unsupportedPlatform: SKError.Code

An error code that indicates the current platform doesn’t support overlays.

### Error domain

let SKErrorDomain: String

The error domain name for StoreKit errors.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

Handling errors

Determine the underlying cause of errors that result from StoreKit requests.

enum Code

Error codes for StoreKit errors.

let SKErrorDomain: String

The error domain name for StoreKit errors.

