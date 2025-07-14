

- Authentication Services
- ASAuthorizationError
-  credentialExport 

Type Property

# credentialExport

The credential export request failed.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
static var credentialExport: ASAuthorizationError.Code { get }
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

static var unknown: ASAuthorizationError.Code

The authorization attempt failed for an unknown reason.

static var credentialImport: ASAuthorizationError.Code

The credential import request failed.

enum Code

Codes that authorization errors can have.

