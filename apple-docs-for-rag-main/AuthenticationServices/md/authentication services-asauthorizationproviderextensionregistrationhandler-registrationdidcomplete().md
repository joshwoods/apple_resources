

- Authentication Services
- ASAuthorizationProviderExtensionRegistrationHandler
-  registrationDidComplete() 

Instance Method

# registrationDidComplete()

Calls the extension to allow it to complete registration.

macOS 13.0+

``` source
optional func registrationDidComplete()
```

## Discussion

The system calls this method once after all current registration calls complete. The extension may free any resources it allocates during registration.

## See Also

### Registering users and devices

func beginDeviceRegistration(loginManager: ASAuthorizationProviderExtensionLoginManager, options: ASAuthorizationProviderExtensionRequestOptions, completion: (ASAuthorizationProviderExtensionRegistrationResult) -> Void)

Initiates the device registration process for the single sign-on extension.

**Required**

func beginUserRegistration(loginManager: ASAuthorizationProviderExtensionLoginManager, userName: String?, method: ASAuthorizationProviderExtensionAuthenticationMethod, options: ASAuthorizationProviderExtensionRequestOptions, completion: (ASAuthorizationProviderExtensionRegistrationResult) -> Void)

Initiates the user registration process for the user and the single sign-on extension.

**Required**

