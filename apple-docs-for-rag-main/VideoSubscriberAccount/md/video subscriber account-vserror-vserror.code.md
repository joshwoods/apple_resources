

- Video Subscriber Account
- VSError
-  VSError.Code 

Enumeration

# VSError.Code

Error codes in the framework error domain.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error Codes

case accessNotGranted

The user hasn’t granted access to their subscription information.

case invalidVerificationToken

The user’s subscription provider rejected the verification token that the app sent with the request.

case providerRejected

The user’s subscription provider didn’t allow the request to proceed.

case rejected

The system rejected the request.

case serviceTemporarilyUnavailable

The request failed due to a timeout or unreachable host, but a subsequent attempt might succeed.

case unsupported

The provider doesn’t support the feature the user requested in the device’s current region.

case unsupportedProvider

The system doesn’t support the user’s subscription provider.

case userCancelled

The user canceled the request.

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

struct VSError

Error information in the framework error domain.

