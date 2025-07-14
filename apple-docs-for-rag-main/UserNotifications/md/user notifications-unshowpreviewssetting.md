

- User Notifications
-  UNShowPreviewsSetting 

Enumeration

# UNShowPreviewsSetting

Constants indicating the style previewing a notification’s content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
enum UNShowPreviewsSetting
```

## Topics

### Preview Styes

case always

The notification’s content is always shown, even when the device is locked.

case whenAuthenticated

The notification’s content is shown only when the device is unlocked.

case never

The notification’s content is never shown, even when the device is unlocked

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Interface Settings

var alertStyle: UNAlertStyle

The type of alert that the app may display when the device is unlocked.

enum UNAlertStyle

Constants indicating the presentation styles for alerts.

var showPreviewsSetting: UNShowPreviewsSetting

The setting that indicates whether the app shows a preview of the notification’s content.

var providesAppNotificationSettings: Bool

A Boolean value indicating the system displays a button for in-app notification settings.

