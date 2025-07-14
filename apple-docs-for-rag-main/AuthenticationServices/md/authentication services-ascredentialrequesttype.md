

- Authentication Services
-  ASCredentialRequestType 

Enumeration

# ASCredentialRequestType

An enumeration that identifies different types of credentials that apps and websites can request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
enum ASCredentialRequestType
```

## Topics

### Credential types

case passkeyAssertion

The app or website is requesting a passkey assertion credential.

case passkeyRegistration

The app or website is requesting a passkey registration credential.

case password

The app or website is requesting a password credential.

case oneTimeCode

The app or website is requesting a one-time passcode.

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

### Identifying the requested credential type

var type: ASCredentialRequestType

The type of credential used for this request.

**Required**

