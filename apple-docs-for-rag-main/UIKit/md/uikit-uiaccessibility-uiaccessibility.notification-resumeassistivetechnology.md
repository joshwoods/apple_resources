

- UIKit
- UIAccessibility
- UIAccessibility.Notification
-  resumeAssistiveTechnology 

Type Property

# resumeAssistiveTechnology

A notification that resumes an assistive app’s operations temporarily.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
nonisolated
static let resumeAssistiveTechnology: UIAccessibility.Notification
```

## Discussion

When posting the notification, specify the assistive app to resume as the parameter. You must post this notification to balance out the previous posting of a pauseAssistiveTechnology notification. Post this notification using the post(notification:argument:) function.

## See Also

### Assistive apps

static let assistiveTouchStatusDidChangeNotification: NSNotification.Name

A notification that indicates a change in the status of AssistiveTouch.

static let guidedAccessStatusDidChangeNotification: NSNotification.Name

A notification that indicates when a Guided Access session starts or ends.

static let pauseAssistiveTechnology: UIAccessibility.Notification

A notification that pauses an assistive app’s operations temporarily.

struct AssistiveTechnologyIdentifier

Identifiers for assistive apps.

