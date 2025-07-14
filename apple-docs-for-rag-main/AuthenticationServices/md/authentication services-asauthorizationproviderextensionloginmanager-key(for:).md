

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  key(for:) 

Instance Method

# key(for:)

Retrieves the key for the specified platform single sign-on key type.

macOS 13.0+

``` source
func key(for keyType: ASAuthorizationProviderExtensionKeyType) -> SecKey?
```

## Parameters 

`keyType`  

The key type to retrieve.

## Return Value

The key identity if it exists, or `nil` if it doesn’t.

## Mentioned in 

Configuring authentication with the identity provider (IdP)

## See Also

### Performing authentication

enum ASAuthorizationProviderExtensionKeyType

The key types for platform single sign-on.

var isDeviceRegistered: Bool

A Boolean value that indicates whether the device completes registration.

var isUserRegistered: Bool

A Boolean value that indicates whether the user completes registration.

var loginConfiguration: ASAuthorizationProviderExtensionLoginConfiguration?

The current login configuration for the extension.

var ssoTokens: [AnyHashable : Any]?

The single sign-on response tokens for the current user and extension.

func identity(for: ASAuthorizationProviderExtensionKeyType) -> SecIdentity?

Retrieves the identity for the specified platform single sign-on key type.

func userNeedsReauthentication(completion: ((any Error)?) -> Void)

Requests platform single sign-on to reauthenticate the current user.

