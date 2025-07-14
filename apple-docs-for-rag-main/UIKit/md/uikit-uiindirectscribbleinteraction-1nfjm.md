

- UIKit
-  UIIndirectScribbleInteraction 

Class

# UIIndirectScribbleInteraction

An interaction for using Scribble to enter text by writing on a view that isn’t formally a text input.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
class UIIndirectScribbleInteraction where Delegate : UIIndirectScribbleInteractionDelegate
```

## Topics

### Creating an indirect Scribble interaction

init(delegate: Delegate)

Creates an indirect Scribble interaction item with the specified delegate.

### Managing indirect Scribble interactions

var delegate: Delegate?

The delegate for the interaction, to supply and customize writable elements in the interaction’s view.

### Detecting writing

var isHandlingWriting: Bool

A Boolean value that indicates whether the user is actively writing.

## Relationships

### Inherits From

- NSObject

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

### Custom views

protocol UIIndirectScribbleInteractionDelegate

Methods that customize behavior on views that aren’t formally text input views.

associatedtype ElementIdentifier : Hashable = String

A unique identifier for a control that isn’t a text field in a Scribble interaction.

**Required**

