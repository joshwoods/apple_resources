

- UIKit
- UIPencilInteraction
- UIPencilInteraction.Tap
-  hoverPose 

Instance Property

# hoverPose

The hover pose of Apple Pencil during a double-tap interaction.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
var hoverPose: UIPencilHoverPose? { get }
```

## Discussion

The value of this property is `nil` if Apple Pencil isn’t close enough to the screen to detect a hover, or if the device doesn’t support hover.

## See Also

### Getting information about a double-tap interaction

var timestamp: TimeInterval

The timestamp of the double-tap interaction.

class UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

