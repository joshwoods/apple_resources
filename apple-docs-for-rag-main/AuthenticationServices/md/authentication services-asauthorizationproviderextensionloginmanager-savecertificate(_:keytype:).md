

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  saveCertificate(\_:keyType:) 

Instance Method

# saveCertificate(\_:keyType:)

Saves the provided certificate for the key type.

macOS 13.0+

``` source
func saveCertificate(
    _ certificate: SecCertificate,
    keyType: ASAuthorizationProviderExtensionKeyType
)
```

## Parameters 

`certificate`  

The certificate to save.

`keyType`  

The key type for the certificate.

## Mentioned in 

Supporting key requests and key exchange requests

Creating and validating a login request

Creating a refresh request

## See Also

### Performing registration

var loginUserName: String?

The user name to use when authenticating with the identity provider.

Deprecated

var registrationToken: String?

The device registration token from the mobile device management profile.

func presentRegistrationViewController(completion: ((any Error)?) -> Void)

Requests platform single sign-on to show the extension’s view controller to the user.

func saveLoginConfiguration(ASAuthorizationProviderExtensionLoginConfiguration) throws

Saves or replaces the login configuration.

