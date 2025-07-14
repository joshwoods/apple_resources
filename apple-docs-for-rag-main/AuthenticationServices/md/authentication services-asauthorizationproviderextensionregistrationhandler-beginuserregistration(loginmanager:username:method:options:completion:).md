

- Authentication Services
- ASAuthorizationProviderExtensionRegistrationHandler
-  beginUserRegistration(loginManager:userName:method:options:completion:) 

Instance Method

# beginUserRegistration(loginManager:userName:method:options:completion:)

Initiates the user registration process for the user and the single sign-on extension.

macOS 13.0+

``` source
func beginUserRegistration(
    loginManager: ASAuthorizationProviderExtensionLoginManager,
    userName: String?,
    method authenticationMethod: ASAuthorizationProviderExtensionAuthenticationMethod,
    options: ASAuthorizationProviderExtensionRequestOptions = [],
    completion: @escaping (ASAuthorizationProviderExtensionRegistrationResult) -> Void
)
```

``` source
func beginUserRegistration(
    loginManager: ASAuthorizationProviderExtensionLoginManager,
    userName: String?,
    method authenticationMethod: ASAuthorizationProviderExtensionAuthenticationMethod,
    options: ASAuthorizationProviderExtensionRequestOptions = []
) async -> ASAuthorizationProviderExtensionRegistrationResult
```

**Required**

## Parameters 

`loginManager`  

The login manager for interfacing with platform SSO.

`userName`  

The user name for the user registration.

`authenticationMethod`  

The authentication method to use for the user.

`options`  

The request options that apply to the request.

`completion`  

The completion to call to continue user registration.

## Mentioned in 

Registering devices and users

## Discussion

The completion handler returns the status as an ASAuthorizationProviderExtensionRegistrationResult.

## See Also

### Registering users and devices

func beginDeviceRegistration(loginManager: ASAuthorizationProviderExtensionLoginManager, options: ASAuthorizationProviderExtensionRequestOptions, completion: (ASAuthorizationProviderExtensionRegistrationResult) -> Void)

Initiates the device registration process for the single sign-on extension.

**Required**

func registrationDidComplete()

Calls the extension to allow it to complete registration.

