

- CloudKit
- CKNotification
-  subscriptionOwnerUserRecordID 

Instance Property

# subscriptionOwnerUserRecordID

The ID of the user record that creates the subscription that generates the push notification.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@NSCopying
var subscriptionOwnerUserRecordID: CKRecord.ID? { get }
```

## Discussion

On a system that supports multiple users, such as tvOS, use this identifier to check whether the pending content is for the current user. If your app always fetches data from CloudKit on launch, you may improve efficiency by disregarding notifications for other users.

For more information about supporting a multiuser environment, see Personalizing Your App for Each User on Apple TV.

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

var subscriptionID: CKSubscription.ID?

The ID of the subscription that triggers the notification.

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

