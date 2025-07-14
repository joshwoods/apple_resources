

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  alertActionLocalizationKey 

Instance Property

# alertActionLocalizationKey

The key that identifies the localized string for the notification’s action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
var alertActionLocalizationKey: String? { get set }
```

## Discussion

Set this property’s value to have the system use a localized string for the text of the notification’s button that opens your app. The system uses the key to find the matching string in your app’s `Localizable.string` file.

If this property’s value is `nil`, the system displays a single button to dismiss the alert.

For information about localizing string resources, see Internationalization and Localization Guide.

## See Also

### Accessing the Notification Alert

var alertBody: String?

The text for the notification’s alert.

var alertLocalizationKey: String?

The key that identifies the localized string for the notification’s alert.

var alertLocalizationArgs: [CKRecord.FieldKey]?

The fields for building a notification’s alert.

var alertLaunchImage: String?

The filename of an image to use as a launch image.

var soundName: String?

The filename of the sound file to play when a notification arrives.

