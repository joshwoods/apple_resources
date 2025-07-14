

- MarketplaceKit
-  InstallConfiguration 

Structure

# InstallConfiguration

Information that describes a requested app installation or app update.

MarketplaceKitUIKitiOS 17.4+iPadOS 17.4+

``` source
struct InstallConfiguration
```

## Overview

The ActionButton.Action.install(_:) enumeration case takes an instance of this structure as a parameter.

## Topics

### Initializers

init(install: InstallMetadata, confirmInstall: () async -> InstallConfirmationResult)

### Instance Properties

let confirmInstall: () async -> InstallConfirmationResult

let install: InstallMetadata

## See Also

### App distribution UI

class ActionButton

A user-interface element that enables a person to install, update, or launch apps by tapping the element.

struct InstallMetadata

Information about a specific app to install or update and the person who initiates it.

enum InstallConfirmationResult

Options that indicate whether the installation of an app proceeds when a person interacts with an app installation button.

struct BatchInstallConfiguration

Information that describes multiple app installations or app updates.

enum BatchInstallConfirmationResult

Options that indicate whether the installation of multiple apps proceeds when a person interacts with an app installation button.

enum MarketplaceDisplayOption

The kinds of deep links that the operating system makes into your marketplace.

protocol MarketplaceSceneDelegate

A delegate that handles deep link requests into your marketplace app.

