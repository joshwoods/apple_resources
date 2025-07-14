

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  titleLocalizationKey 

Instance Property

# titleLocalizationKey

The key that identifies the localized string for the notification’s title.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
var titleLocalizationKey: String? { get set }
```

## Discussion

CloudKit uses this value to set the `title-loc-key` push notification property.

See Generating a remote notification for more details about push notification properties.

## See Also

### Accessing the Notification Title

var title: String?

The notification’s title.

var titleLocalizationArgs: [CKRecord.FieldKey]?

The fields for building a notification’s title.

