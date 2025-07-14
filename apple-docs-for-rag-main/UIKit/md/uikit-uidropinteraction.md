

- UIKit
-  UIDropInteraction 

Class

# UIDropInteraction

An interaction to enable dropping of items onto a view, employing a delegate to instantiate objects and respond to calls from the drop session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDropInteraction
```

## Mentioned in 

Making a view into a drop destination

## Topics

### Initializing drop interactions

init(delegate: any UIDropInteractionDelegate)

Initializes a drop interaction object with a custom delegate object.

### Managing drop interactions

var delegate: (any UIDropInteractionDelegate)?

An object that configures and controls a drop interaction.

protocol UIDropInteractionDelegate

The interface for configuring and controlling a drop interaction.

### Allowing simultaneous drops

var allowsSimultaneousDropSessions: Bool

A Boolean value that specifies whether the drop interaction handles more than one simultaneous drop session.

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

### Drag and drop interactions

protocol UIDragInteractionDelegate

The interface for configuring and controlling a drag interaction.

protocol UIDropInteractionDelegate

The interface for configuring and controlling a drop interaction.

class UIDragInteraction

An interaction to enable dragging of items from a view, employing a delegate to provide drag items and to respond to calls from the drag session.

