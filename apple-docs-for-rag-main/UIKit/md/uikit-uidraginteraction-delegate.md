

- UIKit
- UIDragInteraction
-  delegate 

Instance Property

# delegate

An object that configures and controls a drag interaction.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIDragInteractionDelegate)? { get }
```

## See Also

### Managing drag interactions

var allowsSimultaneousRecognitionDuringLift: Bool

A Boolean value that determines whether the interaction allows recognition of other gestures during the lift activity.

protocol UIDragInteractionDelegate

The interface for configuring and controlling a drag interaction.

