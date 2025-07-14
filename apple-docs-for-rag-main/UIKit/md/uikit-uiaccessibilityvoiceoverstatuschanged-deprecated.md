

- UIKit
-  UIAccessibilityVoiceOverStatusChanged Deprecated

Global Variable

# UIAccessibilityVoiceOverStatusChanged

A notification that UIKit posts when VoiceOver starts or stops.

iOS 4.0–11.0DeprecatediPadOS 4.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–11.0Deprecated

``` source
nonisolated
let UIAccessibilityVoiceOverStatusChanged: String
```

Deprecated

Use voiceOverStatusDidChangeNotification instead.

## Discussion

This notification doesn’t include a parameter.

Use this notification to customize your application’s user interface (UI) for VoiceOver users. For example, if you display a UI element that briefly overlays other parts of your UI, you can make the display persistent for VoiceOver users, but allow it to disappear as designed for users who are not using VoiceOver. You can also use the isVoiceOverRunning function to determine whether VoiceOver is currently running.

Observe this notification using the default notification center.

## See Also

### VoiceOver

static let announcement: UIAccessibility.Notification

A notification that an app posts when it needs to convey an announcement to the assistive app.

static let voiceOverStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when VoiceOver starts or stops.

static let announcementDidFinishNotification: NSNotification.Name

A notification that UIKit posts when the system finishes reading an announcement.

