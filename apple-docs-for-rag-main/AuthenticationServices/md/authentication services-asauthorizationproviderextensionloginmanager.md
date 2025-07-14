

- Authentication Services
-  ASAuthorizationProviderExtensionLoginManager 

Class

# ASAuthorizationProviderExtensionLoginManager

An interface to maintain platform single sign-on (SSO) during authentication and registration.

macOS 13.0+

``` source
class ASAuthorizationProviderExtensionLoginManager
```

## Mentioned in 

Configuring authentication with the identity provider (IdP)

## Overview

Use this class to perform registration and authentication tasks, and to repair registrations.

## Topics

### Performing registration

var loginUserName: String?

The user name to use when authenticating with the identity provider.

Deprecated

var registrationToken: String?

The device registration token from the mobile device management profile.

func presentRegistrationViewController(completion: ((any Error)?) -> Void)

Requests platform single sign-on to show the extension’s view controller to the user.

func saveCertificate(SecCertificate, keyType: ASAuthorizationProviderExtensionKeyType)

Saves the provided certificate for the key type.

func saveLoginConfiguration(ASAuthorizationProviderExtensionLoginConfiguration) throws

Saves or replaces the login configuration.

### Performing authentication

enum ASAuthorizationProviderExtensionKeyType

The key types for platform single sign-on.

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

### Repairing registrations

func userRegistrationsNeedsRepair()

Invokes the user registration to run again so the current user can repair it.

func deviceRegistrationsNeedsRepair()

Invokes the device registration to run again so the current user can repair it.

func resetKeys()

Creates new encryption, signing, and Secure Enclave keys for the user.

### Instance Properties

var extensionData: [AnyHashable : Any]

var userLoginConfiguration: ASAuthorizationProviderExtensionUserLoginConfiguration?

### Instance Methods

func decryptionKeysNeedRepair()

func resetDeviceKeys()

func resetUserSecureEnclaveKey()

func saveUserLoginConfiguration(ASAuthorizationProviderExtensionUserLoginConfiguration) throws

func attestKey(ofType: ASAuthorizationProviderExtensionKeyType, clientDataHash: Data) async throws -> [SecCertificate]

func attestPendingKey(ofType: ASAuthorizationProviderExtensionKeyType, clientDataHash: Data) async throws -> [SecCertificate]

func beginKeyRotation(ASAuthorizationProviderExtensionKeyType) -> SecKey?

func completeKeyRotation(ASAuthorizationProviderExtensionKeyType)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuration

Configuring Device Management

Configure Device Management to support device and user registration for platform SSO.

Configuring authentication with the identity provider (IdP)

Specify how platform SSO authenticates with the identity provider.

class ASAuthorizationProviderExtensionLoginConfiguration

An interface for configuring platform single sign-on.

