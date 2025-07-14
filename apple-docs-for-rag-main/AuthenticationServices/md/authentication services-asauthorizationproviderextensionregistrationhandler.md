

- Authentication Services
-  ASAuthorizationProviderExtensionRegistrationHandler 

Protocol

# ASAuthorizationProviderExtensionRegistrationHandler

An interface through which a single sign-on (SSO) authentication provider extension registers users and devices for platform SSO.

macOS 13.0+

``` source
protocol ASAuthorizationProviderExtensionRegistrationHandler : NSObjectProtocol
```

## Mentioned in 

Registering devices and users

## Topics

### Registering users and devices

func beginDeviceRegistration(loginManager: ASAuthorizationProviderExtensionLoginManager, options: ASAuthorizationProviderExtensionRequestOptions, completion: (ASAuthorizationProviderExtensionRegistrationResult) -> Void)

Initiates the device registration process for the single sign-on extension.

**Required**

func beginUserRegistration(loginManager: ASAuthorizationProviderExtensionLoginManager, userName: String?, method: ASAuthorizationProviderExtensionAuthenticationMethod, options: ASAuthorizationProviderExtensionRequestOptions, completion: (ASAuthorizationProviderExtensionRegistrationResult) -> Void)

Initiates the user registration process for the user and the single sign-on extension.

**Required**

func registrationDidComplete()

Calls the extension to allow it to complete registration.

### Instance Methods

func protocolVersion() -> ASAuthorizationProviderExtensionPlatformSSOProtocolVersion

func registrationDidCancel()

func supportedGrantTypes() -> ASAuthorizationProviderExtensionSupportedGrantTypes

func keyWillRotate(for: ASAuthorizationProviderExtensionKeyType, newKey: SecKey, loginManager: ASAuthorizationProviderExtensionLoginManager, completion: (Bool) -> Void)

### Instance Properties

var supportedDeviceEncryptionAlgorithms: [ASAuthorizationProviderExtensionEncryptionAlgorithm]

var supportedDeviceSigningAlgorithms: [ASAuthorizationProviderExtensionSigningAlgorithm]

var supportedUserSecureEnclaveKeySigningAlgorithms: [ASAuthorizationProviderExtensionSigningAlgorithm]

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Essentials

Creating extensions that support platform SSO

Configure capabilities and authentication options for extensions.

Registering devices and users

Implement device and user registration.

enum ASAuthorizationProviderExtensionAuthenticationMethod

The platform single sign-on method for the user.

struct ASAuthorizationProviderExtensionRequestOptions

The options for the extension to obtain the status of the registration.

enum ASAuthorizationProviderExtensionRegistrationResult

The registration result.

