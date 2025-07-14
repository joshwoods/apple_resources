

- Authentication Services
-  ASAuthorizationProviderExtensionKeyType 

Enumeration

# ASAuthorizationProviderExtensionKeyType

The key types for platform single sign-on.

macOS 13.0+

``` source
enum ASAuthorizationProviderExtensionKeyType
```

## Topics

### Identifying the key types

case userDeviceEncryption

The user device encryption key.

case userDeviceSigning

The user device signing key.

case userSecureEnclaveKey

The user Secure Enclave key.

### Enumeration Cases

case currentDeviceEncryption

case currentDeviceSigning

case sharedDeviceEncryption

case sharedDeviceSigning

case userSmartCard

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

### Performing authentication

var isDeviceRegistered: Bool

A Boolean value that indicates whether the device completes registration.

var isUserRegistered: Bool

A Boolean value that indicates whether the user completes registration.

var loginConfiguration: ASAuthorizationProviderExtensionLoginConfiguration?

The current login configuration for the extension.

var ssoTokens: [AnyHashable : Any]?

The single sign-on response tokens for the current user and extension.

func identity(for: ASAuthorizationProviderExtensionKeyType) -> SecIdentity?

Retrieves the identity for the specified platform single sign-on key type.

func key(for: ASAuthorizationProviderExtensionKeyType) -> SecKey?

Retrieves the key for the specified platform single sign-on key type.

func userNeedsReauthentication(completion: ((any Error)?) -> Void)

Requests platform single sign-on to reauthenticate the current user.

