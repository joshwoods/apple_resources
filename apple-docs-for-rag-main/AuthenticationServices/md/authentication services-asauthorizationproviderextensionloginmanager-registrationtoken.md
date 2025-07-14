

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  registrationToken 

Instance Property

# registrationToken

The device registration token from the mobile device management profile.

macOS 13.0+

``` source
var registrationToken: String? { get }
```

## See Also

### Performing registration

var loginUserName: String?

The user name to use when authenticating with the identity provider.

Deprecated

func presentRegistrationViewController(completion: ((any Error)?) -> Void)

Requests platform single sign-on to show the extension’s view controller to the user.

func saveCertificate(SecCertificate, keyType: ASAuthorizationProviderExtensionKeyType)

Saves the provided certificate for the key type.

func saveLoginConfiguration(ASAuthorizationProviderExtensionLoginConfiguration) throws

Saves or replaces the login configuration.

