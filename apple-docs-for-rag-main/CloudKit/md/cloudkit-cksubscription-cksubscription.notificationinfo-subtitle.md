

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  subtitle 

Instance Property

# subtitle

The notification’s subtitle.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
var subtitle: String? { get set }
```

## Discussion

CloudKit uses this value to set the `subtitle` push notification property. If you set subtitleLocalizationKey, CloudKit ignores this value.

See Generating a remote notification for more details about push notification properties.

## See Also

### Accessing the Notification Subtitle

var subtitleLocalizationKey: String?

The key that identifies the localized string for the notification’s subtitle.

var subtitleLocalizationArgs: [CKRecord.FieldKey]?

The fields for building a notification’s subtitle.

