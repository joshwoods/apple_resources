

- PassKit (Apple Pay and Wallet)
-  PKPassLibraryNotificationKey 

Structure

# PKPassLibraryNotificationKey

The user info keys that a pass library notification uses.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct PKPassLibraryNotificationKey
```

## Topics

### Creating a pass library notification key

init(rawValue: String)

Creates a pass library notification key according to the provided raw value.

### Notification keys

static let addedPassesUserInfoKey: PKPassLibraryNotificationKey

An array of added passes.

static let passTypeIdentifierUserInfoKey: PKPassLibraryNotificationKey

The pass’s pass type identifier.

static let recoveredPassesUserInfoKey: PKPassLibraryNotificationKey

static let removedPassInfosUserInfoKey: PKPassLibraryNotificationKey

An array of dictionaries that describes the removed passes.

static let replacementPassesUserInfoKey: PKPassLibraryNotificationKey

An array of replaced passes.

static let serialNumberUserInfoKey: PKPassLibraryNotificationKey

The pass’s serial number.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Receiving notifications

struct PKPassLibraryNotificationName

The types of notifications that the pass library posts.

