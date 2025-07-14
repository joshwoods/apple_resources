

- Authentication Services
-  ASAuthorizationPlatformPublicKeyCredentialProvider 

Class

# ASAuthorizationPlatformPublicKeyCredentialProvider

A mechanism for providing public key credential requests to an app or service with iCloud Keychain.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
class ASAuthorizationPlatformPublicKeyCredentialProvider
```

## Mentioned in 

Supporting passkeys

## Overview

The credential provider accesses public-private key pairs stored in iCloud Keychain for registration or authentication with a relying party. Instantiate this object, passing in the relying party identifier for the credentials.

## Topics

### Creating the provider

init(relyingPartyIdentifier: String)

Creates the object with a relying party identifier.

### Creating the request

var relyingPartyIdentifier: String

The domain name of the service to register or authorize against.

func createCredentialAssertionRequest(challenge: Data) -> ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

Creates an assertion request with a challenge.

func createCredentialRegistrationRequest(challenge: Data, name: String, userID: Data) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

Creates an assertion request with a challenge, name, and user ID.

### Instance Methods

func createCredentialRegistrationRequest(challenge: Data, name: String, userID: Data, requestStyle: ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest.RequestStyle) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationProvider
- ASAuthorizationWebBrowserPlatformPublicKeyCredentialProvider
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Credential providers

class ASAuthorizationSecurityKeyPublicKeyCredentialProvider

A mechanism for providing public key credential requests to an app or service with a physical security key.

