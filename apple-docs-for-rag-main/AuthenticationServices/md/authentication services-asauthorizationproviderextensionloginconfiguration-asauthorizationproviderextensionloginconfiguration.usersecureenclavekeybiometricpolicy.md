

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  ASAuthorizationProviderExtensionLoginConfiguration.UserSecureEnclaveKeyBiometricPolicy 

Structure

# ASAuthorizationProviderExtensionLoginConfiguration.UserSecureEnclaveKeyBiometricPolicy

macOS 10.15+

``` source
struct UserSecureEnclaveKeyBiometricPolicy
```

## Topics

### Initializers

init(rawValue: UInt)

### Type Properties

static var passwordFallback: ASAuthorizationProviderExtensionLoginConfiguration.UserSecureEnclaveKeyBiometricPolicy

static var reuseDuringUnlock: ASAuthorizationProviderExtensionLoginConfiguration.UserSecureEnclaveKeyBiometricPolicy

static var touchIDOrWatchAny: ASAuthorizationProviderExtensionLoginConfiguration.UserSecureEnclaveKeyBiometricPolicy

static var touchIDOrWatchCurrentSet: ASAuthorizationProviderExtensionLoginConfiguration.UserSecureEnclaveKeyBiometricPolicy

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

### Enumerations

enum FederationType

enum ASAuthorizationProviderExtensionPlatformSSOProtocolVersion

struct ASAuthorizationProviderExtensionSupportedGrantTypes

enum ASAuthorizationPublicKeyCredentialAttachment

struct IdentityTypes

enum ASPublicKeyCredentialClientDataCrossOriginValue

enum ASUserAgeRange

