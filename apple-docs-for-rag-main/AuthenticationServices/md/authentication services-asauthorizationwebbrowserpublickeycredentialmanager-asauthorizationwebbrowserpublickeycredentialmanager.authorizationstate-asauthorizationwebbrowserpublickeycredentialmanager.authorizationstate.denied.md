

- Authentication Services
- ASAuthorizationWebBrowserPublicKeyCredentialManager
- ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState
-  ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState.denied 

Case

# ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState.denied

Someone forbids the browser app to use passkeys stored in the keychain, and managed by third-party credential manager apps.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.4+macOS 13.3+

``` source
case denied
```

## Mentioned in 

Authenticating people by using passkeys in browser apps

## Discussion

The person can change their decision by navigating to Passkeys Access for Web Browsers, in the Privacy & Security pane in Settings.

## See Also

### Passkey access states

case authorized

Someone allows the browser app to use passkeys stored in the keychain, and managed by third-party credential manager apps.

case notDetermined

The person has yet to choose whether to allow the browser app to access passkeys stored on the keychain, or managed by third-party credential managers.

