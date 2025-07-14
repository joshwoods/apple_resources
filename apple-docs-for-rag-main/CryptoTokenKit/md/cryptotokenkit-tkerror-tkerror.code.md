

- CryptoTokenKit
- TKError
-  TKError.Code 

Enumeration

# TKError.Code

Error codes from CryptoTokenKit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Code
```

## Topics

### Error Codes

case notImplemented

The functionality is not implemented.

case communicationError

A communication error occurred.

case corruptedData

The data was corrupted.

case canceledByUser

The operation was canceled by the user.

case authenticationFailed

Authentication failed.

case objectNotFound

The object was not found.

case tokenNotFound

The token was not found.

case badParameter

An invalid parameter was provided.

case authenticationNeeded

Authentication is needed.

static var TKErrorAuthenticationFailed: TKError.CodeDeprecated

static var TKErrorObjectNotFound: TKError.CodeDeprecated

static var TKErrorTokenNotFound: TKError.CodeDeprecated

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

struct TKError

An error specific to the CryptoTokenKit framework.

let TKErrorDomain: String

The domain for all CryptoTokenKit framework errors.

