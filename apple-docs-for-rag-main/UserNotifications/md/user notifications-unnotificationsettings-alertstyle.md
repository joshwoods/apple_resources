

- User Notifications
- UNNotificationSettings
-  alertStyle 

Instance Property

# alertStyle

The type of alert that the app may display when the device is unlocked.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
var alertStyle: UNAlertStyle { get }
```

## Discussion

When alerts are authorized, this property specifies the presentation style for alerts when the device is unlocked. The user may choose to display alerts as automatically disappearing banners or as modal windows that require explicit dismissal. The user may also choose not to display alerts at all.

## See Also

### Getting Interface Settings

enum UNAlertStyle

Constants indicating the presentation styles for alerts.

var showPreviewsSetting: UNShowPreviewsSetting

The setting that indicates whether the app shows a preview of the notification’s content.

enum UNShowPreviewsSetting

Constants indicating the style previewing a notification’s content.

var providesAppNotificationSettings: Bool

A Boolean value indicating the system displays a button for in-app notification settings.

