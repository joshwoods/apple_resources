

- Authentication Services
- ASAuthorizationWebBrowserPublicKeyCredentialManager
-  platformCredentials(forRelyingParty:) 

Instance Method

# platformCredentials(forRelyingParty:)

Gets a list of passkeys available for authenticating with the given relying party.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.4+macOS 13.3+

``` source
func platformCredentials(forRelyingParty relyingParty: String) async -> [ASAuthorizationWebBrowserPlatformPublicKeyCredential]
```

## Parameters 

`relyingParty`  

The name of the relying party, which you receive from the web server that issues the authentication challenge.

## Return Value

A list of credentials stored on the keychain, or managed by third-party credential managers, that are appropriate for responding to the current challenge.

## Discussion

Before calling this method, check that the value of authorizationStateForPlatformCredentials is ASAuthorizationWebBrowserPublicKeyCredentialManager.AuthorizationState.authorized and call requestAuthorizationForPublicKeyCredentials(_:) if your app needs authorization. If you call this method without authorization, it returns an empty array.

## See Also

### Using passkeys

struct ASAuthorizationWebBrowserPlatformPublicKeyCredential

A structure that describes a passkey stored in the keychain, or managed by a third-party credential manager.

