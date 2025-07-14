

- UIKit
- UINotificationFeedbackGenerator
-  UINotificationFeedbackGenerator.FeedbackType 

Enumeration

# UINotificationFeedbackGenerator.FeedbackType

The type of notification that a notification feedback generator object generates.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
enum FeedbackType
```

## Topics

### Constants

case error

A notification feedback type that indicates a task has failed.

case success

A notification feedback type that indicates a task has completed successfully.

case warning

A notification feedback type that indicates a task has produced a warning.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Producing notification feedback

func notificationOccurred(UINotificationFeedbackGenerator.FeedbackType)

Triggers notification feedback.

func notificationOccurred(UINotificationFeedbackGenerator.FeedbackType, at: CGPoint)

Triggers notification feedback at the specified location.

