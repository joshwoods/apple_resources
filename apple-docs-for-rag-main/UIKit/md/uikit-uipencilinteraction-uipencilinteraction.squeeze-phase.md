

- UIKit
- UIPencilInteraction
- UIPencilInteraction.Squeeze
-  phase 

Instance Property

# phase

The phase of a squeeze interaction on Apple Pencil.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
var phase: UIPencilInteraction.Phase { get }
```

## See Also

### Getting information about a squeeze interaction

var timestamp: TimeInterval

The timestamp of the squeeze interaction.

enum Phase

Constants that describe the phases of an interaction on Apple Pencil.

var hoverPose: UIPencilHoverPose?

The hover pose of Apple Pencil during a squeeze interaction.

class UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

