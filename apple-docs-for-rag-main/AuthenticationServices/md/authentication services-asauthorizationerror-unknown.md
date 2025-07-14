

- Authentication Services
- ASAuthorizationError
-  unknown 

Type Property

# unknown

The authorization attempt failed for an unknown reason.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var unknown: ASAuthorizationError.Code { get }
```

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

static var credentialExport: ASAuthorizationError.Code

The credential export request failed.

static var credentialImport: ASAuthorizationError.Code

The credential import request failed.

enum Code

Codes that authorization errors can have.

