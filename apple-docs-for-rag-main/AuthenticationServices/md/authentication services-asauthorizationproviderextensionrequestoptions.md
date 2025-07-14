

- Authentication Services
-  ASAuthorizationProviderExtensionRequestOptions 

Structure

# ASAuthorizationProviderExtensionRequestOptions

The options for the extension to obtain the status of the registration.

macOS 13.0+

``` source
struct ASAuthorizationProviderExtensionRequestOptions
```

## Topics

### Creating the options

init(rawValue: UInt)

Creates the request options.

### Identifying the options

static var registrationRepair: ASAuthorizationProviderExtensionRequestOptions

Indicates that the registration is undergoing repair.

static var userInteractionEnabled: ASAuthorizationProviderExtensionRequestOptions

Indicates that the user interface is in an enabled state.

### Type Properties

static var registrationDeviceKeyMigration: ASAuthorizationProviderExtensionRequestOptions

static var registrationSharedDeviceKeys: ASAuthorizationProviderExtensionRequestOptions

static var userKeyInvalid: ASAuthorizationProviderExtensionRequestOptions

static var strongerKeyAvailable: ASAuthorizationProviderExtensionRequestOptions

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Essentials

Creating extensions that support platform SSO

Configure capabilities and authentication options for extensions.

Registering devices and users

Implement device and user registration.

protocol ASAuthorizationProviderExtensionRegistrationHandler

An interface through which a single sign-on (SSO) authentication provider extension registers users and devices for platform SSO.

enum ASAuthorizationProviderExtensionAuthenticationMethod

The platform single sign-on method for the user.

enum ASAuthorizationProviderExtensionRegistrationResult

The registration result.

