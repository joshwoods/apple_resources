

- Authentication Services
- ASAuthorizationError
-  ASAuthorizationError.Code 

Enumeration

# ASAuthorizationError.Code

Codes that authorization errors can have.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Code
```

## Topics

### Codes

case canceled

The user canceled the authorization attempt.

case failed

The authorization attempt failed.

case invalidResponse

The authorization request received an invalid response.

case notHandled

The authorization request wasn’t handled.

case unknown

The authorization attempt failed for an unknown reason.

case notInteractive

The authorization request isn’t interactive.

case credentialExport

The credential export request failed.

case credentialImport

The credential import request failed.

### Enumeration Cases

case matchedExcludedCredential

This error should only be returned when specifying @c excludedCredentials on a public key credential registration request.

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

### Error Codes

static var canceled: ASAuthorizationError.Code

The user canceled the authorization attempt.

static var failed: ASAuthorizationError.Code

The authorization attempt failed.

static var invalidResponse: ASAuthorizationError.Code

The authorization request received an invalid response.

static var notHandled: ASAuthorizationError.Code

The authorization request wasn’t handled.

static var unknown: ASAuthorizationError.Code

The authorization attempt failed for an unknown reason.

static var credentialExport: ASAuthorizationError.Code

The credential export request failed.

static var credentialImport: ASAuthorizationError.Code

The credential import request failed.

