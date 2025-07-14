

- MarketplaceKit
-  MarketplaceDisplayOption 

Enumeration

# MarketplaceDisplayOption

The kinds of deep links that the operating system makes into your marketplace.

MarketplaceKitUIKitiOS 17.4+iPadOS 17.4+

``` source
enum MarketplaceDisplayOption
```

## Overview

The MarketplaceSceneDelegate function scene(_:askedToDisplay:) accepts a case of this enumeration as a parameter.

## Topics

### Enumeration Cases

case authentication(account: String)

case productPage(appleItemID: AppleItemID, appleVersionID: AppleVersionID?)

case searchResults(query: String)

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

## Relationships

### Conforms To

- Decodable
- Encodable

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

protocol MarketplaceSceneDelegate

A delegate that handles deep link requests into your marketplace app.

