

- MarketplaceKit
-  BatchInstallConfirmationResult 

Enumeration

# BatchInstallConfirmationResult

Options that indicate whether the installation of multiple apps proceeds when a person interacts with an app installation button.

MarketplaceKitUIKitiOS 17.4+iPadOS 17.4+

``` source
enum BatchInstallConfirmationResult
```

## Overview

The BatchInstallConfiguration initializer init(installs:confirmInstall:) takes a closure as a parameter that returns a case of this enumeration.

Your marketplace app supplies code in the closure that facilitates any prerequisites a person needs to satisfy to download the apps, such as completing a payment flow. The result of the prerequisites flow helps you determine the case to return, (BatchInstallConfirmationResult.cancel or BatchInstallConfirmationResult.confirmed(installVerificationTokens:authenticationContext:).

## Topics

### Operators

static func == (BatchInstallConfirmationResult, BatchInstallConfirmationResult) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case cancel

case confirmed(installVerificationTokens: [AppleItemID : String], authenticationContext: LAContext?)

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### App distribution UI

class ActionButton

A user-interface element that enables a person to install, update, or launch apps by tapping the element.

struct InstallMetadata

Information about a specific app to install or update and the person who initiates it.

struct InstallConfiguration

Information that describes a requested app installation or app update.

enum InstallConfirmationResult

Options that indicate whether the installation of an app proceeds when a person interacts with an app installation button.

struct BatchInstallConfiguration

Information that describes multiple app installations or app updates.

enum MarketplaceDisplayOption

The kinds of deep links that the operating system makes into your marketplace.

protocol MarketplaceSceneDelegate

A delegate that handles deep link requests into your marketplace app.

