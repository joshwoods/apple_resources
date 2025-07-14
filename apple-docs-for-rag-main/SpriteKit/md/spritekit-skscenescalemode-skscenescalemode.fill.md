

- SpriteKit
- SKSceneScaleMode
-  SKSceneScaleMode.fill 

Case

# SKSceneScaleMode.fill

Each axis of the scene is scaled independently so that each axis in the scene exactly maps to the length of that axis in the view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+watchOS 2.0+

``` source
case fill
```

## See Also

### Constants

case aspectFill

The scaling factor of each dimension is calculated and the larger of the two is chosen. Each axis of the scene is scaled by the same scaling factor. This guarantees that the entire area of the view is filled but may cause parts of the scene to be cropped.

case aspectFit

The scaling factor of each dimension is calculated and the smaller of the two is chosen. Each axis of the scene is scaled by the same scaling factor. This guarantees that the entire scene is visible but may require letterboxing in the view.

case resizeFill

The scene is not scaled to match the view. Instead, the scene is automatically resized so that its dimensions always match those of the view.

