

- Authentication Services
-  ASAuthorizationProviderExtensionRegistrationResult 

Enumeration

# ASAuthorizationProviderExtensionRegistrationResult

The registration result.

macOS 13.0+

``` source
enum ASAuthorizationProviderExtensionRegistrationResult
```

## Mentioned in 

Registering devices and users

## Topics

### Identifying the results

case failed

The registration fails to complete and the system retries later.

case failedNoRetry

The registration fails to complete and the system doesn’t retry later.

case success

The registration succeeds.

case userInterfaceRequired

The user interface is required to complete registration.

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

enum ASAuthorizationProviderExtensionAuthenticationMethod

The platform single sign-on method for the user.

struct ASAuthorizationProviderExtensionRequestOptions

The options for the extension to obtain the status of the registration.

