

- Foundation
- NSNotification
- NSNotification.Name
-  ALAssetsLibraryChanged Deprecated

Type Property

# ALAssetsLibraryChanged

Sent when the contents of the assets library have changed from under the app that is using the data.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
static let ALAssetsLibraryChanged: NSNotification.Name
```

Deprecated

Use photoLibraryDidChange: notification from the Photos framework instead

## Discussion

In iOS 4.0, the notification’s object is `nil`. In iOS 4.1 and later, the notification object is the library object that posted the notification.

In iOS 6.0 and later, the user information dictionary describes what changed:

- If the user information dictionary is `nil`, reload all assets and asset groups.

- If the user information dictionary an empty dictionary, there is no need to reload assets and asset groups.

- If the user information dictionary is not empty, reload the effected assets and asset groups. For the keys used, see `Notification Keys`.

This notification is sent on an arbitrary thread.

