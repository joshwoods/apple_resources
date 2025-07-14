

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  presentRegistrationViewController(completion:) 

Instance Method

# presentRegistrationViewController(completion:)

Requests platform single sign-on to show the extension’s view controller to the user.

macOS 13.0+

``` source
func presentRegistrationViewController(completion: @escaping ((any Error)?) -> Void)
```

``` source
func presentRegistrationViewController() async throws
```

## Parameters 

`completion`  

A completion handler that the method uses to indicate whether the view controller presents successfully, and the specific error if it doesn’t.

## Mentioned in 

Registering devices and users

## Discussion

This is only valid during registration. If the system can’t show the controller, the completion returns an error.

## See Also

### Performing registration

var loginUserName: String?

The user name to use when authenticating with the identity provider.

Deprecated

var registrationToken: String?

The device registration token from the mobile device management profile.

func saveCertificate(SecCertificate, keyType: ASAuthorizationProviderExtensionKeyType)

Saves the provided certificate for the key type.

func saveLoginConfiguration(ASAuthorizationProviderExtensionLoginConfiguration) throws

Saves or replaces the login configuration.

