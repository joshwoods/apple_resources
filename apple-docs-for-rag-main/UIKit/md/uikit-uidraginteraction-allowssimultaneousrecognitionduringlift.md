

- UIKit
- UIDragInteraction
-  allowsSimultaneousRecognitionDuringLift 

Instance Property

# allowsSimultaneousRecognitionDuringLift

A Boolean value that determines whether the interaction allows recognition of other gestures during the lift activity.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsSimultaneousRecognitionDuringLift: Bool { get set }
```

## Discussion

If you set the allowsSimultaneousRecognitionDuringLift property to true, the interaction is canceled when another gesture is recognized. If you set this property to false (the default value), competing gesture recognizers fail.

Note

UILongPressGestureRecognizer instances are always delayed and happen simultaneously during the lift activity.

## See Also

### Managing drag interactions

var delegate: (any UIDragInteractionDelegate)?

An object that configures and controls a drag interaction.

protocol UIDragInteractionDelegate

The interface for configuring and controlling a drag interaction.

