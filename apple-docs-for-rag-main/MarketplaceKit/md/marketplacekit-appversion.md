

- MarketplaceKit
-  AppVersion 

Structure

# AppVersion

Information that describes an app, including its identifier and version number.

iOS 17.4+iPadOS 17.4+

``` source
struct AppVersion
```

## Overview

Your app’s MarketplaceExtension provides the operating system an instance of this structure when asked via your implementation of the availableAppVersions(forAppleItemIDs:) callback.

## Topics

### Initializers

init(appleItemID: AppleItemID, appleVersionID: UInt64)

### Instance Properties

let appleItemID: AppleItemID

let appleVersionID: UInt64

var description: String

A textual representation of this instance.

## Relationships

### Conforms To

- CustomStringConvertible
- Sendable

## See Also

### App management

class AppLibrary

An object that manages search characteristics, licensing, and the installation of apps.

struct AutomaticUpdate

Information that describes an app that’s available for update, including a download URL.

struct InstallRequirements

An app’s installation criteria for a device.

typealias AppleItemID

An identifier that represents an app.

typealias AppleVersionID

An identifier that represents a single app version.

let MarketplaceKitURIScheme: String

A URI scheme that defines an alternative distribution app installation link.

