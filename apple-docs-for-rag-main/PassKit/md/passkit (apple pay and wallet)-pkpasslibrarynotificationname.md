

- PassKit (Apple Pay and Wallet)
-  PKPassLibraryNotificationName 

Structure

# PKPassLibraryNotificationName

The types of notifications that the pass library posts.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct PKPassLibraryNotificationName
```

## Topics

### Creating a pass library notification name

init(rawValue: String)

Creates a pass library notification name according to the provided raw value.

init(String)

Creates a pass library notification name according to the provided string.

### Notification names

static let PKPassLibraryDidChange: PKPassLibraryNotificationName

A notification that PassKit posts when the pass library changes.

static let PKPassLibraryRemotePaymentPassesDidChange: PKPassLibraryNotificationName

A notification that PassKit posts when it adds or removes a pass on a paired remote device.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Receiving notifications

struct PKPassLibraryNotificationKey

The user info keys that a pass library notification uses.

