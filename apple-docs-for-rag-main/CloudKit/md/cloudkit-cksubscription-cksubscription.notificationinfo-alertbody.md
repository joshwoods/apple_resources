

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  alertBody 

Instance Property

# alertBody

The text for the notification’s alert.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
var alertBody: String? { get set }
```

## Discussion

Set this property’s value to have the system display the specified string when it receives the corresponding push notification. If you localize your app’s content, use the alertLocalizationKey property instead.

## See Also

### Accessing the Notification Alert

var alertLocalizationKey: String?

The key that identifies the localized string for the notification’s alert.

var alertLocalizationArgs: [CKRecord.FieldKey]?

The fields for building a notification’s alert.

var alertActionLocalizationKey: String?

The key that identifies the localized string for the notification’s action.

var alertLaunchImage: String?

The filename of an image to use as a launch image.

var soundName: String?

The filename of the sound file to play when a notification arrives.

