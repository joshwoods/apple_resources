

- Authentication Services
-  ASAuthorizationSecurityKeyPublicKeyCredentialProvider 

Class

# ASAuthorizationSecurityKeyPublicKeyCredentialProvider

A mechanism for providing public key credential requests to an app or service with a physical security key.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class ASAuthorizationSecurityKeyPublicKeyCredentialProvider
```

## Mentioned in 

Supporting Security Key Authentication Using Physical Keys

## Overview

The credential provider accesses public-private key pairs stored on a physical security key for registration or authentication with a relying party. Instantiate this object, passing in the relying party identifier for the credentials.

## Topics

### Creating the provider

init(relyingPartyIdentifier: String)

Creates the object with a relying party identifier.

### Creating the request

var relyingPartyIdentifier: String

The domain name of the service to authorize against.

func createCredentialAssertionRequest(challenge: Data) -> ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

Creates an assertion request with a challenge.

func createCredentialRegistrationRequest(challenge: Data, displayName: String, name: String, userID: Data) -> ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

Creates an assertion request with a challenge, display name, and user ID.

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationProvider
- ASAuthorizationWebBrowserSecurityKeyPublicKeyCredentialProvider
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

class ASAuthorizationPlatformPublicKeyCredentialProvider

A mechanism for providing public key credential requests to an app or service with iCloud Keychain.

