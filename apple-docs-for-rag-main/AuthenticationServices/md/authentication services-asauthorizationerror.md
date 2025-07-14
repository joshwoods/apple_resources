

- Authentication Services
-  ASAuthorizationError 

Structure

# ASAuthorizationError

Errors that can occur during authorization.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ASAuthorizationError
```

## Topics

### Getting the Properties

static var notInteractive: ASAuthorizationError.Code

### Error Domain

let ASAuthorizationErrorDomain: String

The domain of authorization errors.

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

enum Code

Codes that authorization errors can have.

### Type Properties

static var errorDomain: String

static var matchedExcludedCredential: ASAuthorizationError.Code

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Handling Authorization Errors

func authorizationController(controller: ASAuthorizationController, didCompleteWithError: any Error)

Tells the delegate when authorization fails, and provides an error explaining why.

let ASAuthorizationErrorDomain: String

The domain of authorization errors.

