

- StoreKit
- SKError
-  invalidOfferPrice 

Type Property

# invalidOfferPrice

Error code indicating that the price you specified in App Store Connect is no longer valid.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+macOS 10.14.4+tvOS 12.2+visionOS 1.0+watchOS 6.2+

``` source
static var invalidOfferPrice: SKError.Code { get }
```

## Discussion

An offer price can become invalid if you change the price of the base subscription such that it is lower than the offer price. Offers must always represent a discounted price.

## See Also

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

static var invalidSignature: SKError.Code

Error code indicating that the signature in a payment discount is not valid.

static var missingOfferParams: SKError.Code

Error code indicating that parameters are missing in a payment discount.

