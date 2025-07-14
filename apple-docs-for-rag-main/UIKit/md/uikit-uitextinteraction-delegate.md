

- UIKit
- UITextInteraction
-  delegate 

Instance Property

# delegate

The object that receives events from the text interaction.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UITextInteractionDelegate)? { get set }
```

## See Also

### Handling text input and interaction events

var textInput: (any UIResponder &amp; UITextInput)?

The object that interacts with the text input system.

protocol UITextInteractionDelegate

An interface that an object implements to receive information about text interaction events.

