

- Video Subscriber Account
-  VSError 

Structure

# VSError

Error information in the framework error domain.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
struct VSError
```

## Topics

### Error Information

var errorCode: Int

var errorUserInfo: [String : Any]

### Error Codes

static var accessNotGranted: VSError.Code

The user hasn’t granted access to their subscription information.

static var invalidVerificationToken: VSError.Code

The user’s subscription provider rejected the verification token that the app sent with the request.

static var providerRejected: VSError.Code

The user’s subscription provider didn’t allow the request to proceed.

static var rejected: VSError.Code

The system rejected the request.

static var serviceTemporarilyUnavailable: VSError.Code

The request failed due to a timeout or unreachable host, but a subsequent attempt might succeed.

static var unsupported: VSError.Code

The provider doesn’t support the feature the user requested in the device’s current region.

static var unsupportedProvider: VSError.Code

The system doesn’t support the user’s subscription provider.

static var userCancelled: VSError.Code

The user canceled the request.

enum Code

Error codes in the framework error domain.

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

let VSErrorDomain: String

The domain for all errors in the framework.

let VSErrorInfoKeySAMLResponse: String

The subscription provider’s SAML error response.

let VSErrorInfoKeySAMLResponseStatus: String

The subscription provider’s SAML error-response status code.

let VSErrorInfoKeyAccountProviderResponse: String

The account provider’s error-response object.

let VSErrorInfoKeyUnsupportedProviderIdentifier: String

The identifier of the unsupported subscription provider.

enum Code

Error codes in the framework error domain.

