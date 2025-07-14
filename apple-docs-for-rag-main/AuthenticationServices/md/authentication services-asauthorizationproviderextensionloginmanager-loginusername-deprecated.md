

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  loginUserName Deprecated

Instance Property

# loginUserName

The user name to use when authenticating with the identity provider.

macOS 13.0–14.0Deprecated

``` source
var loginUserName: String? { get set }
```

## See Also

### Performing registration

var registrationToken: String?

The device registration token from the mobile device management profile.

func presentRegistrationViewController(completion: ((any Error)?) -> Void)

Requests platform single sign-on to show the extension’s view controller to the user.

func saveCertificate(SecCertificate, keyType: ASAuthorizationProviderExtensionKeyType)

Saves the provided certificate for the key type.

func saveLoginConfiguration(ASAuthorizationProviderExtensionLoginConfiguration) throws

Saves or replaces the login configuration.

