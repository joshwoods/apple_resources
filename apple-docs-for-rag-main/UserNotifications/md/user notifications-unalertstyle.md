

- User Notifications
-  UNAlertStyle 

Enumeration

# UNAlertStyle

Constants indicating the presentation styles for alerts.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
enum UNAlertStyle
```

## Topics

### Presentation Styles

case none

No alert.

case banner

Banner alerts.

case alert

Modal alerts.

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

var showPreviewsSetting: UNShowPreviewsSetting

The setting that indicates whether the app shows a preview of the notification’s content.

enum UNShowPreviewsSetting

Constants indicating the style previewing a notification’s content.

var providesAppNotificationSettings: Bool

A Boolean value indicating the system displays a button for in-app notification settings.

