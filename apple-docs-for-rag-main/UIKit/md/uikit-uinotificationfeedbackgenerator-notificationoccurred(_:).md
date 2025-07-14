

- UIKit
- UINotificationFeedbackGenerator
-  notificationOccurred(\_:) 

Instance Method

# notificationOccurred(\_:)

Triggers notification feedback.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func notificationOccurred(_ notificationType: UINotificationFeedbackGenerator.FeedbackType)
```

## Parameters 

`notificationType`  

The type of notification feedback. For a list of valid notification types, see the UINotificationFeedbackGenerator.FeedbackType enumeration.

## Discussion

This method tells the generator that a task or action has succeeded, failed, or produced a warning. In response, the generator may play the appropriate haptics, based on the provided UINotificationFeedbackGenerator.FeedbackType value.

For more information on setting up a feedback generator, see the UIFeedbackGenerator class.

## See Also

### Related Documentation

func prepare()

Prepares the generator to trigger feedback.

### Producing notification feedback

func notificationOccurred(UINotificationFeedbackGenerator.FeedbackType, at: CGPoint)

Triggers notification feedback at the specified location.

enum FeedbackType

The type of notification that a notification feedback generator object generates.

