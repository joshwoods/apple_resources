

- AppKit
- NSSharingService
- NSSharingService.Name
-  cloudSharing 

Type Property

# cloudSharing

A service that shares an item provider’s contents with other iCloud users.

macOS 10.12+

``` source
static let cloudSharing: NSSharingService.Name
```

## Discussion

The behavior of the cloud-sharing service is different from other services. It creates a persistent sharing session between two or more iCloud users, and provides access to the original items, rather than sending copies. For more information about CloudKit Sharing, see Shared Records.

## See Also

### Sharing Service Names

static let addToAperture: NSSharingService.Name

A service that shares an item provider’s contents with Aperture.

static let addToIPhoto: NSSharingService.Name

A service that shares an item provider’s contents with iPhoto.

static let addToSafariReadingList: NSSharingService.Name

A service that shares an item provider’s contents with Safari’s Reading List.

static let composeEmail: NSSharingService.Name

A service that uses an item provider’s contents to compose an email.

static let composeMessage: NSSharingService.Name

A service that uses an item provider’s contents to compose a message.

static let sendViaAirDrop: NSSharingService.Name

A service that sends an item provider’s contents to another device using AirDrop.

static let useAsDesktopPicture: NSSharingService.Name

A service that sets the item provider’s contents as the current user’s desktop picture.

