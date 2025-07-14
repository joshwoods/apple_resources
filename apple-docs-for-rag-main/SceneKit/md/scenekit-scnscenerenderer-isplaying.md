

- SceneKit
- SCNSceneRenderer
-  isPlaying 

Instance Property

# isPlaying

A Boolean value that determines whether the scene is playing.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isPlaying: Bool { get set }
```

**Required**

## Discussion

If the value of this property is false (the default), SceneKit does not increment the scene time, so animations associated with the scene do not play. Change this property’s value to true to start animating the scene.

## See Also

### Managing Scene Animation Timing

var sceneTime: TimeInterval

The current scene time.

**Required**

var loops: Bool

A Boolean value that determines whether SceneKit restarts the scene time after all animations in the scene have played.

**Required**

