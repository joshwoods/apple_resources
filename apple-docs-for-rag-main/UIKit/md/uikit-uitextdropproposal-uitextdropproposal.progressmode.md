

- UIKit
- UITextDropProposal
-  UITextDropProposal.ProgressMode 

Enumeration

# UITextDropProposal.ProgressMode

The text drop progress styles for user-visible progress indication.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum ProgressMode
```

## Topics

### Progress modes

case custom

A text drop progress mode that indicates that you will provide custom progress indicator during the loading of dropped items.

case system

A text drop progress mode indicating that the system will show the progress indicator.

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

enum Action

The text drop action styles for text views.

enum Performer

The performers that are responsible for handling the drop operation.

