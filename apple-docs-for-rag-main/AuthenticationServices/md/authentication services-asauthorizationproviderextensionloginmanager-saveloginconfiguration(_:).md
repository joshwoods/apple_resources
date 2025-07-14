

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  saveLoginConfiguration(\_:) 

Instance Method

# saveLoginConfiguration(\_:)

Saves or replaces the login configuration.

macOS 13.0+

``` source
func saveLoginConfiguration(_ loginConfiguration: ASAuthorizationProviderExtensionLoginConfiguration) throws
```

## Parameters 

`loginConfiguration`  

The login configuration to save or replace.

## See Also

### Performing registration

var loginUserName: String?

The user name to use when authenticating with the identity provider.

Deprecated

var registrationToken: String?

The device registration token from the mobile device management profile.

func presentRegistrationViewController(completion: ((any Error)?) -> Void)

Requests platform single sign-on to show the extension’s view controller to the user.

func saveCertificate(SecCertificate, keyType: ASAuthorizationProviderExtensionKeyType)

Saves the provided certificate for the key type.

