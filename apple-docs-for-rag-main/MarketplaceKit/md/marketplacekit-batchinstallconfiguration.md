

- MarketplaceKit
-  BatchInstallConfiguration 

Structure

# BatchInstallConfiguration

Information that describes multiple app installations or app updates.

MarketplaceKitUIKitiOS 17.4+iPadOS 17.4+

``` source
struct BatchInstallConfiguration
```

## Overview

The ActionButton.Action.batchInstall(_:) enumeration case takes an instance of this structure as a parameter.

## Topics

### Initializers

init(installs: [InstallMetadata], confirmInstall: () async -> BatchInstallConfirmationResult)

### Instance Properties

let confirmInstall: () async -> BatchInstallConfirmationResult

let installs: [InstallMetadata]

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

enum BatchInstallConfirmationResult

Options that indicate whether the installation of multiple apps proceeds when a person interacts with an app installation button.

enum MarketplaceDisplayOption

The kinds of deep links that the operating system makes into your marketplace.

protocol MarketplaceSceneDelegate

A delegate that handles deep link requests into your marketplace app.

