

- Authentication Services
-  ASAccountAuthenticationModificationRequest 

Class

# ASAccountAuthenticationModificationRequest

A request to modify an account’s authentication properties.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class ASAccountAuthenticationModificationRequest
```

## Overview

To initiate an account authentication modification request from your app, use either ASAccountAuthenticationModificationUpgradePasswordToStrongPasswordRequest or ASAccountAuthenticationModificationReplacePasswordWithSignInWithAppleRequest.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ASAccountAuthenticationModificationReplacePasswordWithSignInWithAppleRequest
- ASAccountAuthenticationModificationUpgradePasswordToStrongPasswordRequest

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

class ASAccountAuthenticationModificationUpgradePasswordToStrongPasswordRequest

A request to automatically upgrade from a weak password to a strong password.

