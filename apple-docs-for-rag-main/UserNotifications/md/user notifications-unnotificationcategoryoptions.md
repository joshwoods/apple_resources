

- User Notifications
-  UNNotificationCategoryOptions 

Structure

# UNNotificationCategoryOptions

Constants indicating how to handle notifications associated with this category.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
struct UNNotificationCategoryOptions
```

## Topics

### Creating an option

init(rawValue: UInt)

Initializes a notification category options object using the specified raw value.

### Customizing a category

static var allowInCarPlay: UNNotificationCategoryOptions

Allow CarPlay to display notifications of this type.

static var allowAnnouncement: UNNotificationCategoryOptions

An option that grants Siri permission to read incoming messages out loud when the user has a compatible audio output device connected.

Deprecated

### Managing hidden preview behavior

static var hiddenPreviewsShowTitle: UNNotificationCategoryOptions

Show the notification’s title, even if the user has disabled notification previews for the app.

static var hiddenPreviewsShowSubtitle: UNNotificationCategoryOptions

Show the notification’s subtitle, even if the user has disabled notification previews for the app.

### Managing action handling behavior

static var customDismissAction: UNNotificationCategoryOptions

Send dismiss actions to the `UNUserNotificationCenter` object’s delegate for handling.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting the Options

var options: UNNotificationCategoryOptions

Options for how to handle notifications of this type.

