

- UIKit
-  UITextInteractionDelegate 

Protocol

# UITextInteractionDelegate

An interface that an object implements to receive information about text interaction events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextInteractionDelegate : NSObjectProtocol
```

## Topics

### Handling text interaction events

func interactionShouldBegin(UITextInteraction, at: CGPoint) -> Bool

Asks the delegate whether the text interaction should begin.

func interactionWillBegin(UITextInteraction)

Tells the delegate that the text interaction will begin.

func interactionDidEnd(UITextInteraction)

Tells the delegate that the text interaction ended.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Text interactions

class UITextInteraction

An interaction that provides text selection gestures and UI to custom text views.

enum UITextInteractionMode

Modes that determine the selection behaviors that a text interaction provides.

