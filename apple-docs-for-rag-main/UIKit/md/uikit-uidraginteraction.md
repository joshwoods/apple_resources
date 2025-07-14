

- UIKit
-  UIDragInteraction 

Class

# UIDragInteraction

An interaction to enable dragging of items from a view, employing a delegate to provide drag items and to respond to calls from the drag session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDragInteraction
```

## Mentioned in 

Making a view into a drag source

## Topics

### Initializing the drag interaction

init(delegate: any UIDragInteractionDelegate)

Initializes a drag interaction object with a custom delegate object.

### Managing drag interactions

var allowsSimultaneousRecognitionDuringLift: Bool

A Boolean value that determines whether the interaction allows recognition of other gestures during the lift activity.

var delegate: (any UIDragInteractionDelegate)?

An object that configures and controls a drag interaction.

protocol UIDragInteractionDelegate

The interface for configuring and controlling a drag interaction.

### Enabling the interactions

var isEnabled: Bool

A Boolean value that specifies whether the drag interaction responds to touches and is allowed to participate in a drag activity.

class var isEnabledByDefault: Bool

A device-dependent Boolean value that indicates whether a newly-instantiated drag interaction is allowed to participate in a drag activity.

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

class UIDropInteraction

An interaction to enable dropping of items onto a view, employing a delegate to instantiate objects and respond to calls from the drop session.

