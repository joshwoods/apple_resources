

- UIKit
-  UIDropSessionProgressIndicatorStyle 

Enumeration

# UIDropSessionProgressIndicatorStyle

The drop-progress indicator styles for the drop session, used while data is moving from the source to the destination.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum UIDropSessionProgressIndicatorStyle
```

## Topics

### Progress indicator styles

case `default`

The indicator style for using the system’s default drop-progress indication.

case none

The indicator style for no drop-progress indication.

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

enum UIDropOperation

Operation types that determine how a drag and drop activity resolves when the user drops a drag item.

