

- Authentication Services
- ASAccountAuthenticationModificationController
-  perform(\_:) 

Instance Method

# perform(\_:)

Performs a request to upgrade the authentication credentials for an account to a strong password, or to use Sign in with Apple.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func perform(_ request: ASAccountAuthenticationModificationRequest)
```

## Parameters 

`request`  

The request to perform.

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Discussion

Only one request can be in progress at a time. If a request is already in progress, additional requests fail immediately.

## See Also

### Initiating Security Upgrades from Your App

class ASAccountAuthenticationModificationReplacePasswordWithSignInWithAppleRequest

A request to upgrade from using a password to using Sign in with Apple.

class ASAccountAuthenticationModificationUpgradePasswordToStrongPasswordRequest

A request to automatically upgrade from a weak password to a strong password.

class ASAccountAuthenticationModificationRequest

A request to modify an account’s authentication properties.

