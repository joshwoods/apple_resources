

- MarketplaceKit
-  MarketplaceSceneDelegate 

Protocol

# MarketplaceSceneDelegate

A delegate that handles deep link requests into your marketplace app.

MarketplaceKitUIKitiOS 17.4+iPadOS 17.4+

``` source
protocol MarketplaceSceneDelegate
```

## Overview

The operating system calls your app’s scene delegate to launch your app to a specific screen, such as a search result or specific app page. The display option argument determines the specific screen.

## Topics

### Instance Methods

func scene(UIWindowScene, askedToDisplay: MarketplaceDisplayOption)

**Required**

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

enum BatchInstallConfirmationResult

Options that indicate whether the installation of multiple apps proceeds when a person interacts with an app installation button.

enum MarketplaceDisplayOption

The kinds of deep links that the operating system makes into your marketplace.

