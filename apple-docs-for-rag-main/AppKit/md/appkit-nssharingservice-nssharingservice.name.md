

- AppKit
- NSSharingService
-  NSSharingService.Name 

Structure

# NSSharingService.Name

Constants that describe the sharing services that macOS supports.

macOS

``` source
struct Name
```

## Topics

### Creating a Sharing Service Name

init(String)

Creates a sharing service name using the provided string.

init(rawValue: String)

Creates a sharing service name using the specified raw value.

### Sharing Service Names

static let addToAperture: NSSharingService.Name

A service that shares an item provider’s contents with Aperture.

static let addToIPhoto: NSSharingService.Name

A service that shares an item provider’s contents with iPhoto.

static let addToSafariReadingList: NSSharingService.Name

A service that shares an item provider’s contents with Safari’s Reading List.

static let cloudSharing: NSSharingService.Name

A service that shares an item provider’s contents with other iCloud users.

static let composeEmail: NSSharingService.Name

A service that uses an item provider’s contents to compose an email.

static let composeMessage: NSSharingService.Name

A service that uses an item provider’s contents to compose a message.

static let sendViaAirDrop: NSSharingService.Name

A service that sends an item provider’s contents to another device using AirDrop.

static let useAsDesktopPicture: NSSharingService.Name

A service that sets the item provider’s contents as the current user’s desktop picture.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Sharing Service

init?(named: NSSharingService.Name)

Returns a sharing service instance representing the specified service name.

init(title: String, image: NSImage, alternateImage: NSImage?, handler: () -> Void)

Creates a custom sharing service object.

