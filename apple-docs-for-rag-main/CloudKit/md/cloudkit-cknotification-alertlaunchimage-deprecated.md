

- CloudKit
- CKNotification
-  alertLaunchImage Deprecated

Instance Property

# alertLaunchImage

The filename of an image to use as a launch image.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.10–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
var alertLaunchImage: String? { get }
```

Deprecated

Interact with UI elements of a CloudKit-server-generated push message via UserNotifications.framework

## Discussion

The system uses this property’s value to locate an image in the app’s bundle, and displays it as a launch image when the user launches the app after receiving a push notification.

## See Also

### Accessing the Notification Info

var alertBody: String?

The notification’s alert body.

Deprecated

var alertLocalizationKey: String?

The key that identifies the localized text for the alert body.

Deprecated

var alertLocalizationArgs: [String]?

The fields for building a notification’s alert.

Deprecated

var alertActionLocalizationKey: String?

The key that identifies the localized string for the notification’s action.

Deprecated

var soundName: String?

The name of the sound file to play when a notification arrives.

Deprecated

var badge: NSNumber?

The value that the app icon’s badge displays.

Deprecated

var category: String?

The name of the action group that corresponds to this notification.

Deprecated

var subscriptionID: CKSubscription.ID?

The ID of the subscription that triggers the notification.

var subscriptionOwnerUserRecordID: CKRecord.ID?

The ID of the user record that creates the subscription that generates the push notification.

var title: String?

The notification’s title.

Deprecated

var titleLocalizationKey: String?

The key that identifies the localized string for the notification’s title.

Deprecated

var titleLocalizationArgs: [String]?

The fields for building a notification’s title.

Deprecated

var subtitle: String?

The notification’s subtitle.

Deprecated

var subtitleLocalizationKey: String?

The key that identifies the localized string for the notification’s subtitle.

Deprecated

var subtitleLocalizationArgs: [String]?

The fields for building a notification’s subtitle.

Deprecated

