

- CloudKit
- CKNotification
-  subscriptionID 

Instance Property

# subscriptionID

The ID of the subscription that triggers the notification.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
var subscriptionID: CKSubscription.ID? { get }
```

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

var alertLaunchImage: String?

The filename of an image to use as a launch image.

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

