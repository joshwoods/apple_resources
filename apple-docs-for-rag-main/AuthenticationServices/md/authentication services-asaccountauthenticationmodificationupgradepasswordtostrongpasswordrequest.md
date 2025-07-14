

- Authentication Services
-  ASAccountAuthenticationModificationUpgradePasswordToStrongPasswordRequest 

Class

# ASAccountAuthenticationModificationUpgradePasswordToStrongPasswordRequest

A request to automatically upgrade from a weak password to a strong password.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class ASAccountAuthenticationModificationUpgradePasswordToStrongPasswordRequest
```

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Overview

Your app uses this class to initiate an upgrade from a weak password to a strong system-generated one. After creating the request, your app initiates the upgrade process by instantiating an ASAccountAuthenticationModificationController object and calling perform(_:) on it. The system invokes your authentication modification extension to complete the upgrade.

For details about how to enforce requirements on the password, such as minimum length or requiring both letters and numbers, see ASAccountAuthenticationModificationPasswordGenerationRequirements.

## Topics

### Creating Upgrade Requests in Your App

init(user: String, serviceIdentifier: ASCredentialServiceIdentifier, userInfo: [AnyHashable : Any]?)

Creates a request to upgrade from using a weak password to using a strong system-generated password.

var user: String

The user name of the account to upgrade.

var serviceIdentifier: ASCredentialServiceIdentifier

An identifier that represents a particular service that the user needs a credential for, like a web site.

var userInfo: [AnyHashable : Any]?

A dictionary that contains values to pass to your account modification extension.

## Relationships

### Inherits From

- ASAccountAuthenticationModificationRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Initiating Security Upgrades from Your App

func perform(ASAccountAuthenticationModificationRequest)

Performs a request to upgrade the authentication credentials for an account to a strong password, or to use Sign in with Apple.

class ASAccountAuthenticationModificationReplacePasswordWithSignInWithAppleRequest

A request to upgrade from using a password to using Sign in with Apple.

class ASAccountAuthenticationModificationRequest

A request to modify an account’s authentication properties.

