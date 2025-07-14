

- MarketplaceKit
-  InstallRequirements 

Structure

# InstallRequirements

An app’s installation criteria for a device.

iOS 17.4+iPadOS 17.4+

``` source
struct InstallRequirements
```

## Topics

### Initializers

init()

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var ageRatingRank: Int?

var expectedInstallSize: UInt64?

var minimumSystemVersion: String?

A text representation of the system version required to install an app.

var requiredDeviceCapabilities: Set&lt;String>?

The capabilities that a device requires to install an app.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func satisfiedByDevice() -> Bool

## Relationships

### Conforms To

- Decodable
- Encodable
- Sendable

## See Also

### App management

class AppLibrary

An object that manages search characteristics, licensing, and the installation of apps.

struct AppVersion

Information that describes an app, including its identifier and version number.

struct AutomaticUpdate

Information that describes an app that’s available for update, including a download URL.

typealias AppleItemID

An identifier that represents an app.

typealias AppleVersionID

An identifier that represents a single app version.

let MarketplaceKitURIScheme: String

A URI scheme that defines an alternative distribution app installation link.

