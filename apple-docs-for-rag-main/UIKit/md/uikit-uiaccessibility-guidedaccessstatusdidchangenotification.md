

- UIKit
- UIAccessibility
-  guidedAccessStatusDidChangeNotification 

Type Property

# guidedAccessStatusDidChangeNotification

A notification that indicates when a Guided Access session starts or ends.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let guidedAccessStatusDidChangeNotification: NSNotification.Name
```

## Discussion

This notification doesn’t include a parameter. Observe this notification using the default notification center.

Use the isGuidedAccessEnabled function to determine whether a Guided Access session is currently active.

## See Also

### Assistive apps

static let assistiveTouchStatusDidChangeNotification: NSNotification.Name

A notification that indicates a change in the status of AssistiveTouch.

static let pauseAssistiveTechnology: UIAccessibility.Notification

A notification that pauses an assistive app’s operations temporarily.

static let resumeAssistiveTechnology: UIAccessibility.Notification

A notification that resumes an assistive app’s operations temporarily.

struct AssistiveTechnologyIdentifier

Identifiers for assistive apps.

