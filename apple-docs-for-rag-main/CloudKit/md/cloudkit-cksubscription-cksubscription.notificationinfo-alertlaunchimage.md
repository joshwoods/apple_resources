

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  alertLaunchImage 

Instance Property

# alertLaunchImage

The filename of an image to use as a launch image.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
var alertLaunchImage: String? { get set }
```

## Discussion

If you specify a value, the system uses it to locate an image in the app’s bundle, and displays it as a launch image when the user launches the app after receiving a push notification.

## See Also

### Accessing the Notification Alert

var alertBody: String?

The text for the notification’s alert.

var alertLocalizationKey: String?

The key that identifies the localized string for the notification’s alert.

var alertLocalizationArgs: [CKRecord.FieldKey]?

The fields for building a notification’s alert.

var alertActionLocalizationKey: String?

The key that identifies the localized string for the notification’s action.

var soundName: String?

The filename of the sound file to play when a notification arrives.

