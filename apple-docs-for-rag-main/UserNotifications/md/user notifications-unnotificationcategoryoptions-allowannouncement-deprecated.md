

- User Notifications
- UNNotificationCategoryOptions
-  allowAnnouncement Deprecated

Type Property

# allowAnnouncement

An option that grants Siri permission to read incoming messages out loud when the user has a compatible audio output device connected.

iOS 13.0–15.0DeprecatediPadOS 13.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 6.0–7.0Deprecated

``` source
static var allowAnnouncement: UNNotificationCategoryOptions { get }
```

Deprecated

Announcement option is ignored

## Discussion

When Siri reads an incoming message to the user, Siri reads the message locally on the userʼs device. Siri doesn’t send the message’s contents or sender to Apple servers. For more information about Siri’s on-device processing, visit Apple’s Privacy Page.

## See Also

### Customizing a category

static var allowInCarPlay: UNNotificationCategoryOptions

Allow CarPlay to display notifications of this type.

