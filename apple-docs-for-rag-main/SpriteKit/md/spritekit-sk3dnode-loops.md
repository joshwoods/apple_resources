

- SpriteKit
- SK3DNode
-  loops 

Instance Property

# loops

A Boolean value that determines whether Scene Kit restarts the scene time after all animations in the scene have played.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var loops: Bool { get set }
```

**watchOS**

``` source
var loops: Bool { get set }
```

## Discussion

If the value of this property is true (the default), SceneKit returns the scene time to zero after all animations associated with the scene have played, causing those animations to repeat. Otherwise, SceneKit stops playing the scene when all animations have completed.

## See Also

### Animating a 3D Node’s Content in Scene Kit

var isPlaying: Bool

A Boolean value that determines whether the scene is playing.

var sceneTime: TimeInterval

The current scene time.

