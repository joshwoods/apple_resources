

- UIKit
-  UIDropOperation 

Enumeration

# UIDropOperation

Operation types that determine how a drag and drop activity resolves when the user drops a drag item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum UIDropOperation
```

## Mentioned in 

Making a view into a drop destination

## Topics

### Drop operation types

case cancel

A drop operation type specifying that no data should be transferred, thereby canceling the drag.

case forbidden

A drop operation type specifying that, although a move or copy operation is typically legitimate in this scenario, the drop activity isn’t allowed.

case copy

A drop operation type specifying that the data represented by the drag items should be copied to the destination view.

case move

A drop operation type specifying that the data represented by the drag items should be moved, not copied.

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

### Drop destinations

protocol UIDropSession

The interface for querying a drop session about its state and associated drag items.

class UIDropProposal

A configuration for the behavior of a drop interaction, required if a view accepts drop activities.

enum UIDropSessionProgressIndicatorStyle

The drop-progress indicator styles for the drop session, used while data is moving from the source to the destination.

