

- SceneKit
- SCNSceneRenderer
-  loops 

Instance Property

# loops

A Boolean value that determines whether SceneKit restarts the scene time after all animations in the scene have played.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var loops: Bool { get set }
```

**Required**

## Discussion

If the value of this property is true (the default), SceneKit returns the scene time to zero after all animations associated with the scene have played, causing those animations to repeat. Otherwise, SceneKit stops playing the scene when all animations have completed.

## See Also

### Managing Scene Animation Timing

var sceneTime: TimeInterval

The current scene time.

**Required**

var isPlaying: Bool

A Boolean value that determines whether the scene is playing.

**Required**

