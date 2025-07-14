

- UIKit
- UIAccessibility
-  assistiveTouchStatusDidChangeNotification 

Type Property

# assistiveTouchStatusDidChangeNotification

A notification that indicates a change in the status of AssistiveTouch.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
nonisolated
static let assistiveTouchStatusDidChangeNotification: NSNotification.Name
```

## Discussion

The user must enable Guided Access for this notification to post.

## See Also

### Assistive apps

static let guidedAccessStatusDidChangeNotification: NSNotification.Name

A notification that indicates when a Guided Access session starts or ends.

static let pauseAssistiveTechnology: UIAccessibility.Notification

A notification that pauses an assistive app’s operations temporarily.

static let resumeAssistiveTechnology: UIAccessibility.Notification

A notification that resumes an assistive app’s operations temporarily.

struct AssistiveTechnologyIdentifier

Identifiers for assistive apps.

