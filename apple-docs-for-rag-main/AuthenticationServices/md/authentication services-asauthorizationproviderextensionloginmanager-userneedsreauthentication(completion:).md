

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  userNeedsReauthentication(completion:) 

Instance Method

# userNeedsReauthentication(completion:)

Requests platform single sign-on to reauthenticate the current user.

macOS 13.0+

``` source
func userNeedsReauthentication(completion: @escaping ((any Error)?) -> Void)
```

``` source
func userNeedsReauthentication() async throws
```

## Parameters 

`completion`  

The completion with the error, if any.

## Discussion

Use this method to request reauthentication, such as when revoking or expiring tokens.

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

func key(for: ASAuthorizationProviderExtensionKeyType) -> SecKey?

Retrieves the key for the specified platform single sign-on key type.

