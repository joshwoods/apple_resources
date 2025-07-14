

- SpriteKit
- SK3DNode
-  isPlaying 

Instance Property

# isPlaying

A Boolean value that determines whether the scene is playing.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var isPlaying: Bool { get set }
```

**watchOS**

``` source
var isPlaying: Bool { get set }
```

## Discussion

If the value of this property is false (the default), SceneKit does not increment the scene time, so animations associated with the scene do not play. Change this property’s value to true to start animating the scene.

## See Also

### Animating a 3D Node’s Content in Scene Kit

var loops: Bool

A Boolean value that determines whether Scene Kit restarts the scene time after all animations in the scene have played.

var sceneTime: TimeInterval

The current scene time.

