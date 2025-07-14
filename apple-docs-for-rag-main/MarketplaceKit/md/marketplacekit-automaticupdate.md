

- MarketplaceKit
-  AutomaticUpdate 

Structure

# AutomaticUpdate

Information that describes an app that’s available for update, including a download URL.

iOS 17.4+iPadOS 17.4+

``` source
struct AutomaticUpdate
```

## Overview

Your app’s MarketplaceExtension provides the operating system an instance of this structure when asked via your implementation of the automaticUpdates(for:) callback.

## Topics

### Initializers

init(appleItemID: AppleItemID, alternativeDistributionPackage: URL, account: String, installVerificationToken: String)

### Instance Properties

let account: String

let alternativeDistributionPackage: URL

var appShareURL: URL?

let appleItemID: AppleItemID

let installVerificationToken: String

## Relationships

### Conforms To

- Sendable

## See Also

### App management

class AppLibrary

An object that manages search characteristics, licensing, and the installation of apps.

struct AppVersion

Information that describes an app, including its identifier and version number.

struct InstallRequirements

An app’s installation criteria for a device.

typealias AppleItemID

An identifier that represents an app.

typealias AppleVersionID

An identifier that represents a single app version.

let MarketplaceKitURIScheme: String

A URI scheme that defines an alternative distribution app installation link.

