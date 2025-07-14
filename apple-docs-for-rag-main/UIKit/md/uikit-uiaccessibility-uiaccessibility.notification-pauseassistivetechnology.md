

- UIKit
- UIAccessibility
- UIAccessibility.Notification
-  pauseAssistiveTechnology 

Type Property

# pauseAssistiveTechnology

A notification that pauses an assistive app’s operations temporarily.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
nonisolated
static let pauseAssistiveTechnology: UIAccessibility.Notification
```

## Discussion

When posting the notification, specify the assistive app to pause as the parameter. For example, you might want to pause scanning in Switch Control while your app is playing an animation. You must balance this notification by posting a resumeAssistiveTechnology notification to resume the assistive app’s operations. Post this notification using the post(notification:argument:) function.

## See Also

### Assistive apps

static let assistiveTouchStatusDidChangeNotification: NSNotification.Name

A notification that indicates a change in the status of AssistiveTouch.

static let guidedAccessStatusDidChangeNotification: NSNotification.Name

A notification that indicates when a Guided Access session starts or ends.

static let resumeAssistiveTechnology: UIAccessibility.Notification

A notification that resumes an assistive app’s operations temporarily.

struct AssistiveTechnologyIdentifier

Identifiers for assistive apps.

