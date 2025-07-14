

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  isUserRegistered 

Instance Property

# isUserRegistered

A Boolean value that indicates whether the user completes registration.

macOS 13.0+

``` source
var isUserRegistered: Bool { get }
```

## Discussion

Returns true if the user completes registration.

## See Also

### Performing authentication

enum ASAuthorizationProviderExtensionKeyType

The key types for platform single sign-on.

var isDeviceRegistered: Bool

A Boolean value that indicates whether the device completes registration.

var loginConfiguration: ASAuthorizationProviderExtensionLoginConfiguration?

The current login configuration for the extension.

var ssoTokens: [AnyHashable : Any]?

The single sign-on response tokens for the current user and extension.

func identity(for: ASAuthorizationProviderExtensionKeyType) -> SecIdentity?

Retrieves the identity for the specified platform single sign-on key type.

func key(for: ASAuthorizationProviderExtensionKeyType) -> SecKey?

Retrieves the key for the specified platform single sign-on key type.

func userNeedsReauthentication(completion: ((any Error)?) -> Void)

Requests platform single sign-on to reauthenticate the current user.

