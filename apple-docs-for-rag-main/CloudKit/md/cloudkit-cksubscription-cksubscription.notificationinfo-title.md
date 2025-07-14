

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  title 

Instance Property

# title

The notification’s title.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
var title: String? { get set }
```

## Discussion

CloudKit uses this value to set the `title` push notification property.

See Generating a remote notification for more detail about push notification properties.

## See Also

### Accessing the Notification Title

var titleLocalizationKey: String?

The key that identifies the localized string for the notification’s title.

var titleLocalizationArgs: [CKRecord.FieldKey]?

The fields for building a notification’s title.

