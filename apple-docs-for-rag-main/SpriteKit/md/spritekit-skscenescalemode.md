

- SpriteKit
-  SKSceneScaleMode 

Enumeration

# SKSceneScaleMode

The modes that determine how the scene’s area is mapped to the view that presents it.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum SKSceneScaleMode
```

## Topics

### Constants

case fill

Each axis of the scene is scaled independently so that each axis in the scene exactly maps to the length of that axis in the view.

case aspectFill

The scaling factor of each dimension is calculated and the larger of the two is chosen. Each axis of the scene is scaled by the same scaling factor. This guarantees that the entire area of the view is filled but may cause parts of the scene to be cropped.

case aspectFit

The scaling factor of each dimension is calculated and the smaller of the two is chosen. Each axis of the scene is scaled by the same scaling factor. This guarantees that the entire scene is visible but may require letterboxing in the view.

case resizeFill

The scene is not scaled to match the view. Instead, the scene is automatically resized so that its dimensions always match those of the view.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Stretching Content to Fit the View

Scaling a Scene’s Content to Fit the View

Configure the scale mode to determine how a scene is sized to fit its view.

var scaleMode: SKSceneScaleMode

A setting that defines how the scene is mapped to the view that presents it.

