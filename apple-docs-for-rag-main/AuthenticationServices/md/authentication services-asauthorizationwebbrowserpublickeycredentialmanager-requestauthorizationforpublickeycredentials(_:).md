

- Authentication Services
- ASAuthorizationWebBrowserPublicKeyCredentialManager
-  requestAuthorizationForPublicKeyCredentials(\_:) 

Instance Method

# requestAuthorizationForPublicKeyCredentials(\_:)

Requests a person’s permission to use their passkeys.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.4+macOS 13.3+

``` source
func requestAuthorizationForPublicKeyCredentials(_ completionHandler: @escaping (ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState) -> Void)
```

``` source
func requestAuthorizationForPublicKeyCredentials() async -> ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState
```

## Parameters 

`completionHandler`  

A block you provide that the operating system calls when the request is completed.

## Mentioned in 

Authenticating people by using passkeys in browser apps

## See Also

### Requesting access to passkeys

var authorizationStateForPlatformCredentials: ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState

Returns a value that indicates whether the browser app has access to a person’s passkeys.

enum AuthorizationState

An enumeration of values that indicate whether the browser app has access to a person’s passkeys.

