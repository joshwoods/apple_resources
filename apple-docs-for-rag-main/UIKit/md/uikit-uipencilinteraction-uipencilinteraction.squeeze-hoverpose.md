

- UIKit
- UIPencilInteraction
- UIPencilInteraction.Squeeze
-  hoverPose 

Instance Property

# hoverPose

The hover pose of Apple Pencil during a squeeze interaction.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
var hoverPose: UIPencilHoverPose? { get }
```

## Discussion

The value of this property is `nil` if Apple Pencil isn’t close enough to the screen to detect a hover, or if the device doesn’t support hover.

## See Also

### Getting information about a squeeze interaction

var timestamp: TimeInterval

The timestamp of the squeeze interaction.

var phase: UIPencilInteraction.Phase

The phase of a squeeze interaction on Apple Pencil.

enum Phase

Constants that describe the phases of an interaction on Apple Pencil.

class UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

