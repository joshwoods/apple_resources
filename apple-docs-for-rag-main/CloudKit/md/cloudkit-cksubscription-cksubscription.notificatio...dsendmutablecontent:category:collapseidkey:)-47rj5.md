

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  init(alertBody:alertLocalizationKey:alertLocalizationArgs:title:titleLocalizationKey:titleLocalizationArgs:subtitle:subtitleLocalizationKey:subtitleLocalizationArgs:alertActionLocalizationKey:alertLaunchImage:soundName:desiredKeys:shouldBadge:shouldSendContentAvailable:shouldSendMutableContent:category:collapseIDKey:) 

Initializer

# init(alertBody:alertLocalizationKey:alertLocalizationArgs:title:titleLocalizationKey:titleLocalizationArgs:subtitle:subtitleLocalizationKey:subtitleLocalizationArgs:alertActionLocalizationKey:alertLaunchImage:soundName:desiredKeys:shouldBadge:shouldSendContentAvailable:shouldSendMutableContent:category:collapseIDKey:)

Creates a notification with the specified values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 6.0+

``` source
convenience init(
    alertBody: String? = nil,
    alertLocalizationKey: String? = nil,
    alertLocalizationArgs: [CKRecord.FieldKey] = [],
    title: String? = nil,
    titleLocalizationKey: String? = nil,
    titleLocalizationArgs: [CKRecord.FieldKey] = [],
    subtitle: String? = nil,
    subtitleLocalizationKey: String? = nil,
    subtitleLocalizationArgs: [CKRecord.FieldKey] = [],
    alertActionLocalizationKey: String? = nil,
    alertLaunchImage: String? = nil,
    soundName: String? = nil,
    desiredKeys: [CKRecord.FieldKey] = [],
    shouldBadge: Bool = false,
    shouldSendContentAvailable: Bool = false,
    shouldSendMutableContent: Bool = false,
    category: String? = nil,
    collapseIDKey: String? = nil
)
```

## Parameters 

`alertBody`  

The text for the notification’s alert.

`alertLocalizationKey`  

The key that identifies the localized string for the notification’s alert.

`alertLocalizationArgs`  

The fields for building a notification’s alert.

`title`  

The notification’s title.

`titleLocalizationKey`  

The key that identifies the localized string for the notification’s title.

`titleLocalizationArgs`  

The fields for building a notification’s title.

`subtitle`  

The notification’s subtitle.

`subtitleLocalizationKey`  

The key that identifies the localized string for the notification’s subtitle.

`subtitleLocalizationArgs`  

The fields for building a notification’s subtitle.

`alertActionLocalizationKey`  

The key that identifies the localized string for the notification’s action.

`alertLaunchImage`  

The filename of an image to use as a launch image.

`soundName`  

The filename of the sound file to play when a notification arrives.

`desiredKeys`  

The names of fields to include in the push notification’s payload.

`shouldBadge`  

A Boolean value that determines whether an app’s icon badge increments its value.

`shouldSendContentAvailable`  

A Boolean value that indicates whether the push notification includes the content available flag.

`shouldSendMutableContent`  

A Boolean value that indicates whether the push notification includes the content available flag.

`category`  

The name of the action group that corresponds to this notification.

`collapseIDKey`  

The value that the system uses to coalesce unseen push notifications.

## Discussion

See the corresponding properties for more details about each parameter.

