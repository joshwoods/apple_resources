

- UIKit
- UINotificationFeedbackGenerator
-  notificationOccurred(\_:at:) 

Instance Method

# notificationOccurred(\_:at:)

Triggers notification feedback at the specified location.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
func notificationOccurred(
    _ notificationType: UINotificationFeedbackGenerator.FeedbackType,
    at location: CGPoint
)
```

## See Also

### Producing notification feedback

func notificationOccurred(UINotificationFeedbackGenerator.FeedbackType)

Triggers notification feedback.

enum FeedbackType

The type of notification that a notification feedback generator object generates.

