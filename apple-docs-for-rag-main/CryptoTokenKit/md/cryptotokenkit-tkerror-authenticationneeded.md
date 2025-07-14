

- CryptoTokenKit
- TKError
-  authenticationNeeded 

Type Property

# authenticationNeeded

Authentication is needed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var authenticationNeeded: TKError.Code { get }
```

## See Also

### Checking Error Codes

static var notImplemented: TKError.Code

The system doesn’t implement the requested functionality.

static var communicationError: TKError.Code

The system had a communication error.

static var corruptedData: TKError.Code

The system idenfitied the data as corrupted.

static var canceledByUser: TKError.Code

The user canceled the operation.

static var authenticationFailed: TKError.Code

Authentication failed.

static var objectNotFound: TKError.Code

The system didn’t find the object.

static var tokenNotFound: TKError.Code

The system didn’t find the token.

static var badParameter: TKError.Code

An invalid parameter was provided.

static var TKErrorAuthenticationFailed: TKError.CodeDeprecated

static var TKErrorObjectNotFound: TKError.CodeDeprecated

static var TKErrorTokenNotFound: TKError.CodeDeprecated

