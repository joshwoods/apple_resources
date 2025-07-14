

- MarketplaceKit
-  InstallMetadata 

Structure

# InstallMetadata

Information about a specific app to install or update and the person who initiates it.

MarketplaceKitUIKitiOS 17.4+iPadOS 17.4+

``` source
struct InstallMetadata
```

## Mentioned in 

Ingesting an alternative distribution package

## Topics

### Initializers

init(account: String, appleItemID: AppleItemID, alternativeDistributionPackage: URL, isUpdate: Bool)

### Instance Properties

let account: String

A user ID for the person installing the app.

let alternativeDistributionPackage: URL

A URL to the app’s assembled alternative distribution package.

var appShareURL: URL?

A URL to a product landing page for the app on your marketplace website.

let appleItemID: AppleItemID

let isUpdate: Bool

## Relationships

### Conforms To

- Sendable

## See Also

### App distribution UI

class ActionButton

A user-interface element that enables a person to install, update, or launch apps by tapping the element.

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

protocol MarketplaceSceneDelegate

A delegate that handles deep link requests into your marketplace app.

