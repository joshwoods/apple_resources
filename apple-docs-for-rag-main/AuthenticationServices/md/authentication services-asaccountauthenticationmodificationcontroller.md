

- Authentication Services
-  ASAccountAuthenticationModificationController 

Class

# ASAccountAuthenticationModificationController

An object that performs a request to modify an account’s authentication properties.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class ASAccountAuthenticationModificationController
```

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Overview

Note

This class ignores calls from Mac apps built with Mac Catalyst.

## Topics

### Initiating Security Upgrades from Your App

func perform(ASAccountAuthenticationModificationRequest)

Performs a request to upgrade the authentication credentials for an account to a strong password, or to use Sign in with Apple.

class ASAccountAuthenticationModificationReplacePasswordWithSignInWithAppleRequest

A request to upgrade from using a password to using Sign in with Apple.

class ASAccountAuthenticationModificationUpgradePasswordToStrongPasswordRequest

A request to automatically upgrade from a weak password to a strong password.

class ASAccountAuthenticationModificationRequest

A request to modify an account’s authentication properties.

### Configuring Requests

var presentationContextProvider: (any ASAccountAuthenticationModificationControllerPresentationContextProviding)?

An object that provides a presentation context for the account modification request’s user interface.

var delegate: (any ASAccountAuthenticationModificationControllerDelegate)?

An object that receives notifications about the request’s status.

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

### Automatic security upgrades

Upgrading Account Security With an Account Authentication Modification Extension

Automatically and transparently convert accounts to Sign in with Apple or to use strong passwords for improved security.

class ASAccountAuthenticationModificationViewController

A view controller that can upgrade user passwords to strong passwords, or convert accounts to use Sign in with Apple.

class ASAccountAuthenticationModificationExtensionContext

An object that you interact with to change an account’s password or to upgrade to Sign in with Apple.

