

- PassKit (Apple Pay and Wallet)
- PKPassLibraryNotificationName
-  PKPassLibraryDidChange 

Type Property

# PKPassLibraryDidChange

A notification that PassKit posts when the pass library changes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
static let PKPassLibraryDidChange: PKPassLibraryNotificationName
```

## Discussion

PassKit posts this notification on an arbitary queue, and only does so if an instance of `PKPassLibrary` exists. The notification’s user info dictionary describes the changes. See PKPassLibrary for the keys it uses.

## See Also

### Notification names

static let PKPassLibraryRemotePaymentPassesDidChange: PKPassLibraryNotificationName

A notification that PassKit posts when it adds or removes a pass on a paired remote device.

