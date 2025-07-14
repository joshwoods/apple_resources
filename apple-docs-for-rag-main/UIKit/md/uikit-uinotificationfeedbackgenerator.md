

- UIKit
-  UINotificationFeedbackGenerator 

Class

# UINotificationFeedbackGenerator

A concrete feedback generator subclass that creates haptics to communicate successes, failures, and warnings.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
class UINotificationFeedbackGenerator
```

## Overview

Use notification feedback to communicate that a task or action succeeded, failed, or produced a warning of some kind.

For more information, read Playing haptic feedback in your app.

## Topics

### Producing notification feedback

func notificationOccurred(UINotificationFeedbackGenerator.FeedbackType)

Triggers notification feedback.

func notificationOccurred(UINotificationFeedbackGenerator.FeedbackType, at: CGPoint)

Triggers notification feedback at the specified location.

enum FeedbackType

The type of notification that a notification feedback generator object generates.

## Relationships

### Inherits From

- UIFeedbackGenerator

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIInteraction

## See Also

### Haptic feedback

Playing haptic feedback in your app

Provide tactile feedback when people perform certain actions in your app.

class UIFeedbackGenerator

The abstract superclass for all feedback generators.

class UIImpactFeedbackGenerator

A concrete feedback generator subclass that creates haptics to simulate physical impacts.

class UISelectionFeedbackGenerator

A concrete feedback generator subclass that creates haptics to indicate a change in selection.

class UICanvasFeedbackGenerator

A concrete feedback generator subclass that creates haptics to indicate events on a drawing canvas.

