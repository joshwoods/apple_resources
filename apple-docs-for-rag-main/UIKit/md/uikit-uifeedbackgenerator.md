

- UIKit
-  UIFeedbackGenerator 

Class

# UIFeedbackGenerator

The abstract superclass for all feedback generators.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
class UIFeedbackGenerator
```

## Overview

Don’t subclass or create instances of this class yourself. Instead, instantiate one of the concrete feedback generator subclasses:

- UIImpactFeedbackGenerator. Use impact feedback to indicate when an impact occurs. For example, you might trigger impact feedback when a user interface object collides with something or snaps into place.

- UISelectionFeedbackGenerator. Use selection feedback to indicate a change in selection.

- UINotificationFeedbackGenerator. Use notification feedback to indicate successes, failures, and warnings.

- UICanvasFeedbackGenerator. Use canvas feedback to indicate when a drawing event occurs, such as an object snapping to a guide or ruler.

For more information, read Playing haptic feedback in your app.

## Topics

### Initializing a feedback generator

convenience init(view: UIView)

Creates a feedback generator and attaches it to the specified view.

### Preparing to generate feedback

func prepare()

Prepares the generator to trigger feedback.

### Deprecated

init()

Creates a feedback generator.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- UICanvasFeedbackGenerator
- UIImpactFeedbackGenerator
- UINotificationFeedbackGenerator
- UISelectionFeedbackGenerator

### Conforms To

- CVarArg
- Copyable
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

class UIImpactFeedbackGenerator

A concrete feedback generator subclass that creates haptics to simulate physical impacts.

class UINotificationFeedbackGenerator

A concrete feedback generator subclass that creates haptics to communicate successes, failures, and warnings.

class UISelectionFeedbackGenerator

A concrete feedback generator subclass that creates haptics to indicate a change in selection.

class UICanvasFeedbackGenerator

A concrete feedback generator subclass that creates haptics to indicate events on a drawing canvas.

