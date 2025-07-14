

- Authentication Services
-  ASAuthorizationWebBrowserPublicKeyCredentialManager 

Class

# ASAuthorizationWebBrowserPublicKeyCredentialManager

A class that you use to request access to a person’s passkeys in a web browser, and that reports on the access status.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.4+macOS 13.3+

``` source
class ASAuthorizationWebBrowserPublicKeyCredentialManager
```

## Mentioned in 

Authenticating people by using passkeys in browser apps

## Topics

### Creating credential managers

init()

Initializes a credential manager.

### Requesting access to passkeys

var authorizationStateForPlatformCredentials: ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState

Returns a value that indicates whether the browser app has access to a person’s passkeys.

func requestAuthorizationForPublicKeyCredentials((ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState) -> Void)

Requests a person’s permission to use their passkeys.

enum AuthorizationState

An enumeration of values that indicate whether the browser app has access to a person’s passkeys.

### Using passkeys

func platformCredentials(forRelyingParty: String) async -> [ASAuthorizationWebBrowserPlatformPublicKeyCredential]

Gets a list of passkeys available for authenticating with the given relying party.

struct ASAuthorizationWebBrowserPlatformPublicKeyCredential

A structure that describes a passkey stored in the keychain, or managed by a third-party credential manager.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Website authorization

Authenticating people by using passkeys in browser apps

Provide a secure and convenient alternative to passwords.

