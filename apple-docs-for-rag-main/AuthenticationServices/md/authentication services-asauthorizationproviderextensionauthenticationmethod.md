

- Authentication Services
-  ASAuthorizationProviderExtensionAuthenticationMethod 

Enumeration

# ASAuthorizationProviderExtensionAuthenticationMethod

The platform single sign-on method for the user.

macOS 13.0+

``` source
enum ASAuthorizationProviderExtensionAuthenticationMethod
```

## Topics

### Identifying the methods

case password

Password authentication.

case userSecureEnclaveKey

Secure Enclave key authentication.

### Enumeration Cases

case smartCard

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Essentials

Creating extensions that support platform SSO

Configure capabilities and authentication options for extensions.

Registering devices and users

Implement device and user registration.

protocol ASAuthorizationProviderExtensionRegistrationHandler

An interface through which a single sign-on (SSO) authentication provider extension registers users and devices for platform SSO.

struct ASAuthorizationProviderExtensionRequestOptions

The options for the extension to obtain the status of the registration.

enum ASAuthorizationProviderExtensionRegistrationResult

The registration result.

