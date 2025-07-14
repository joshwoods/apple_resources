

- Authentication Services
- ASAuthorizationProviderExtensionRegistrationHandler
-  beginDeviceRegistration(loginManager:options:completion:) 

Instance Method

# beginDeviceRegistration(loginManager:options:completion:)

Initiates the device registration process for the single sign-on extension.

macOS 13.0+

``` source
func beginDeviceRegistration(
    loginManager: ASAuthorizationProviderExtensionLoginManager,
    options: ASAuthorizationProviderExtensionRequestOptions = [],
    completion: @escaping (ASAuthorizationProviderExtensionRegistrationResult) -> Void
)
```

``` source
func beginDeviceRegistration(
    loginManager: ASAuthorizationProviderExtensionLoginManager,
    options: ASAuthorizationProviderExtensionRequestOptions = []
) async -> ASAuthorizationProviderExtensionRegistrationResult
```

**Required**

## Parameters 

`loginManager`  

The login manager for interfacing with platform SSO.

`options`  

The request options that apply to the request.

`completion`  

The completion to call to continue device registration.

## Mentioned in 

Registering devices and users

## Discussion

The completion handler returns the status as an ASAuthorizationProviderExtensionRegistrationResult.

## See Also

### Registering users and devices

func beginUserRegistration(loginManager: ASAuthorizationProviderExtensionLoginManager, userName: String?, method: ASAuthorizationProviderExtensionAuthenticationMethod, options: ASAuthorizationProviderExtensionRequestOptions, completion: (ASAuthorizationProviderExtensionRegistrationResult) -> Void)

Initiates the user registration process for the user and the single sign-on extension.

**Required**

func registrationDidComplete()

Calls the extension to allow it to complete registration.

