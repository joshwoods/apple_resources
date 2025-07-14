

- Authentication Services
- ASAuthorizationWebBrowserPublicKeyCredentialManager
-  authorizationStateForPlatformCredentials 

Instance Property

# authorizationStateForPlatformCredentials

Returns a value that indicates whether the browser app has access to a person’s passkeys.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.4+macOS 13.3+

``` source
var authorizationStateForPlatformCredentials: ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState { get }
```

## Mentioned in 

Authenticating people by using passkeys in browser apps

## See Also

### Requesting access to passkeys

func requestAuthorizationForPublicKeyCredentials((ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState) -> Void)

Requests a person’s permission to use their passkeys.

enum AuthorizationState

An enumeration of values that indicate whether the browser app has access to a person’s passkeys.

