

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  soundName 

Instance Property

# soundName

The filename of the sound file to play when a notification arrives.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
var soundName: String? { get set }
```

## Discussion

If you specify a value, the system uses it to locate a sound file in the app’s bundle. The sound plays when the system receives a push notification. If the system can’t find the specified file, or if you use the string `default`, the system plays the default sound.

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

var alertLaunchImage: String?

The filename of an image to use as a launch image.

