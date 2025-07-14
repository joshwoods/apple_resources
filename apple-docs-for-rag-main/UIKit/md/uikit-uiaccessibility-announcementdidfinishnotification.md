

- UIKit
- UIAccessibility
-  announcementDidFinishNotification 

Type Property

# announcementDidFinishNotification

A notification that UIKit posts when the system finishes reading an announcement.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
nonisolated
static let announcementDidFinishNotification: NSNotification.Name
```

## Discussion

The parameter is a dictionary with two keys, announcementStringValueUserInfoKey and announcementWasSuccessfulUserInfoKey. Observe this notification using the default notification center.

## See Also

### VoiceOver

static let announcement: UIAccessibility.Notification

A notification that an app posts when it needs to convey an announcement to the assistive app.

static let voiceOverStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when VoiceOver starts or stops.

let UIAccessibilityVoiceOverStatusChanged: String

A notification that UIKit posts when VoiceOver starts or stops.

Deprecated

