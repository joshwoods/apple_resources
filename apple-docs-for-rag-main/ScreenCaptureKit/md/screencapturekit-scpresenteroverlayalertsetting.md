

- ScreenCaptureKit
-  SCPresenterOverlayAlertSetting 

Enumeration

# SCPresenterOverlayAlertSetting

Configures how to present streaming notifications to a streamer of Presenter Overlay.

Mac Catalyst 18.2+macOS 14.0+

``` source
enum SCPresenterOverlayAlertSetting
```

## Topics

### Alerting Presenters

case always

Always display an alert when using Presenter Overlay.

case never

Never display an alert when using Presenter Overlay.

case system

Displays an alert when using Presenter Overlay based on the System Settings.

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

### Notifying presenters

var presenterOverlayPrivacyAlertSetting: SCPresenterOverlayAlertSetting

A value indicating if alerts appear to presenters while using Presenter Overlay.

