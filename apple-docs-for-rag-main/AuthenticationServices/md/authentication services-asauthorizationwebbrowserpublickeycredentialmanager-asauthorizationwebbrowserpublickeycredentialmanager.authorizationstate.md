

- Authentication Services
- ASAuthorizationWebBrowserPublicKeyCredentialManager
-  ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState 

Enumeration

# ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState

An enumeration of values that indicate whether the browser app has access to a person’s passkeys.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.4+macOS 13.3+

``` source
enum AuthorizationState
```

## Topics

### Passkey access states

case authorized

Someone allows the browser app to use passkeys stored in the keychain, and managed by third-party credential manager apps.

case denied

Someone forbids the browser app to use passkeys stored in the keychain, and managed by third-party credential manager apps.

case notDetermined

The person has yet to choose whether to allow the browser app to access passkeys stored on the keychain, or managed by third-party credential managers.

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

### Requesting access to passkeys

var authorizationStateForPlatformCredentials: ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState

Returns a value that indicates whether the browser app has access to a person’s passkeys.

func requestAuthorizationForPublicKeyCredentials((ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState) -> Void)

Requests a person’s permission to use their passkeys.

