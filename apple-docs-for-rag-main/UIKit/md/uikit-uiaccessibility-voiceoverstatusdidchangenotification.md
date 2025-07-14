

- UIKit
- UIAccessibility
-  voiceOverStatusDidChangeNotification 

Type Property

# voiceOverStatusDidChangeNotification

A notification that UIKit posts when VoiceOver starts or stops.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
nonisolated
static let voiceOverStatusDidChangeNotification: NSNotification.Name
```

## Discussion

Use this notification to customize your app’s UI for VoiceOver users. For example, if you display a UI element that briefly overlays other parts of your UI, you can make the display persistent for VoiceOver users, but allow it to not appear for users who aren’t using VoiceOver. You can also use the isVoiceOverRunning function to determine whether VoiceOver is currently running.

Observe this notification using the default notification center. This notification doesn’t include a parameter.

## See Also

### VoiceOver

static let announcement: UIAccessibility.Notification

A notification that an app posts when it needs to convey an announcement to the assistive app.

static let announcementDidFinishNotification: NSNotification.Name

A notification that UIKit posts when the system finishes reading an announcement.

let UIAccessibilityVoiceOverStatusChanged: String

A notification that UIKit posts when VoiceOver starts or stops.

Deprecated

