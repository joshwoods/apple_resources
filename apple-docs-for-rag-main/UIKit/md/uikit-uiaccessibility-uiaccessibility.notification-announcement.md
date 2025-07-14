

- UIKit
- UIAccessibility
- UIAccessibility.Notification
-  announcement 

Type Property

# announcement

A notification that an app posts when it needs to convey an announcement to the assistive app.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
nonisolated
static let announcement: UIAccessibility.Notification
```

## Discussion

This notification includes a parameter that is an NSString object that contains the announcement. An assistive app outputs the announcement string in the parameter.

Use this notification to provide accessibility information about events that don’t update the app’s UI, or that update the UI only briefly.

Post this notification using the post(notification:argument:) function.

## See Also

### VoiceOver

static let voiceOverStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when VoiceOver starts or stops.

static let announcementDidFinishNotification: NSNotification.Name

A notification that UIKit posts when the system finishes reading an announcement.

let UIAccessibilityVoiceOverStatusChanged: String

A notification that UIKit posts when VoiceOver starts or stops.

Deprecated

