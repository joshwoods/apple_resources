

- UIKit
-  UITextDropProposal 

Class

# UITextDropProposal

A proposed configuration for the behavior of a text drop interaction.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UITextDropProposal
```

## Topics

### Configuring a text drop proposal

var dropAction: UITextDropProposal.Action

A text drop action style that specifies how the text view receives dropped items.

enum Action

The text drop action styles for text views.

var dropPerformer: UITextDropProposal.Performer

The performer that is responsible for handling the drop operation.

enum Performer

The performers that are responsible for handling the drop operation.

var dropProgressMode: UITextDropProposal.ProgressMode

A mode that specifies how the text view indicates progress to the user when loading dropped items.

enum ProgressMode

The text drop progress styles for user-visible progress indication.

var useFastSameViewOperations: Bool

A Boolean value that determines whether the text view can use fast inline dropping when the source and destination are in the same text view.

## Relationships

### Inherits From

- UIDropProposal

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Drop management

protocol UITextDropRequest

The interface for specifying the attributes of a drop request for a text view.

enum Action

The text drop action styles for text views.

enum Performer

The performers that are responsible for handling the drop operation.

enum ProgressMode

The text drop progress styles for user-visible progress indication.

