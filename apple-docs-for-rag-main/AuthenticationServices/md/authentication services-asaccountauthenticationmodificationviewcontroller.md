

- Authentication Services
-  ASAccountAuthenticationModificationViewController 

Class

# ASAccountAuthenticationModificationViewController

A view controller that can upgrade user passwords to strong passwords, or convert accounts to use Sign in with Apple.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
class ASAccountAuthenticationModificationViewController
```

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Overview

Adding an account modification extension lets your app seamlessly upgrade user passwords to strong passwords, or convert from using passwords to using Sign in with Apple. The entire process can be automatic, requiring no user interaction, or you can include interactions, such as two-factor authentication confirmation.

Note

This class ignores calls from Mac apps built with Mac Catalyst.

## Topics

### Upgrading to Sign in with Apple

func convertAccountToSignInWithAppleWithoutUserInteraction(for: ASCredentialServiceIdentifier, existingCredential: ASPasswordCredential, userInfo: [AnyHashable : Any]?)

Converts an account’s authentication mechanism from using passwords to using Sign in with Apple.

func prepareInterfaceToConvertAccountToSignInWithApple(for: ASCredentialServiceIdentifier, existingCredential: ASPasswordCredential, userInfo: [AnyHashable : Any]?)

Prepares the view controller’s interface that displays when converting an account that uses password authentication to use Sign in with Apple.

ASAccountAuthenticationModificationSupportsUpgradeToSignInWithApple

A Boolean value that indicates whether the extension supports upgrading from using password authentication to using Sign in with Apple.

### Upgrading to Strong Passwords

func changePasswordWithoutUserInteraction(for: ASCredentialServiceIdentifier, existingCredential: ASPasswordCredential, newPassword: String, userInfo: [AnyHashable : Any]?)

Upgrades a user’s weak password to a strong password.

func prepareInterfaceToChangePassword(for: ASCredentialServiceIdentifier, existingCredential: ASPasswordCredential, newPassword: String, userInfo: [AnyHashable : Any]?)

Prepares the view controller’s interface that displays when upgrading from a weak password to a strong password.

ASAccountAuthenticationModificationSupportsStrongPasswordChange

A Boolean value that indicates whether the extension supports upgrading a user’s password to a strong password.

ASAccountAuthenticationModificationPasswordGenerationRequirements

The rules the system satisfies when generating a strong password for your extension during an automatic upgrade.

ASAccountAuthenticationModificationOptOutOfSecurityPromptsOnSignIn

A Boolean value that indicates the system shouldn’t show security recommendation prompts when users sign in using the app.

### Handling Modification Requests

func cancelRequest()

Cancels a request that the user initiated.

protocol ASAccountAuthenticationModificationControllerDelegate

An interface you implement for receiving success and failure statuses about modification of an account’s authentication properties.

protocol ASAccountAuthenticationModificationControllerPresentationContextProviding

An interface you implement to coordinate presentation of the user interface when modifying an account’s authentication properties.

### Getting the Extension Context

var extensionContext: ASAccountAuthenticationModificationExtensionContext

The context your account authentication modification extension uses to provide information to the system.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Automatic security upgrades

Upgrading Account Security With an Account Authentication Modification Extension

Automatically and transparently convert accounts to Sign in with Apple or to use strong passwords for improved security.

class ASAccountAuthenticationModificationController

An object that performs a request to modify an account’s authentication properties.

class ASAccountAuthenticationModificationExtensionContext

An object that you interact with to change an account’s password or to upgrade to Sign in with Apple.

