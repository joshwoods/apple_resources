

- UIKit
- UITextDropProposal
-  UITextDropProposal.Action 

Enumeration

# UITextDropProposal.Action

The text drop action styles for text views.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Action
```

## Topics

### Text drop actions

case insert

A text drop action style specifying that text is inserted at the provided location, without altering the surrounding text.

case replaceAll

A text drop action style specifying that the dropped text replaces all text in the target text view.

case replaceSelection

A text drop action style specifying that if the target text view contains a selection, dropped text replaces it.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Drop management

protocol UITextDropRequest

The interface for specifying the attributes of a drop request for a text view.

class UITextDropProposal

A proposed configuration for the behavior of a text drop interaction.

enum Performer

The performers that are responsible for handling the drop operation.

enum ProgressMode

The text drop progress styles for user-visible progress indication.

