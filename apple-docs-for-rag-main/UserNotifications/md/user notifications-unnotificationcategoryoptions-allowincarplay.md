

- User Notifications
- UNNotificationCategoryOptions
-  allowInCarPlay 

Type Property

# allowInCarPlay

Allow CarPlay to display notifications of this type.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 3.0+

``` source
static var allowInCarPlay: UNNotificationCategoryOptions { get }
```

## Discussion

Apps must be approved for CarPlay overall and then you must enable CarPlay for the notification types you want displayed. If a category doesn’t explicitly contain this option, notifications of that type aren’t displayed in a CarPlay environment.

## See Also

### Customizing a category

static var allowAnnouncement: UNNotificationCategoryOptions

An option that grants Siri permission to read incoming messages out loud when the user has a compatible audio output device connected.

Deprecated

