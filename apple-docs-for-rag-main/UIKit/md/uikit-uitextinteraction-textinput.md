

- UIKit
- UITextInteraction
-  textInput 

Instance Property

# textInput

The object that interacts with the text input system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var textInput: (any UIResponder & UITextInput)? { get set }
```

## Discussion

The object that you assign to textInput can be different than the view that contains the text interaction. For example, you may want the gestures for the text interaction to work on a container view, such as a scroll view, while managing the text selection behavior in a contained view, such as the one drawing the text.

## See Also

### Handling text input and interaction events

var delegate: (any UITextInteractionDelegate)?

The object that receives events from the text interaction.

protocol UITextInteractionDelegate

An interface that an object implements to receive information about text interaction events.

