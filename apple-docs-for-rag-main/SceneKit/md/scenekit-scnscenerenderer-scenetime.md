

- SceneKit
- SCNSceneRenderer
-  sceneTime 

Instance Property

# sceneTime

The current scene time.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var sceneTime: TimeInterval { get set }
```

**Required**

## Discussion

This timestamp determines how running animations behave, which is similar to how the playhead time in a video player application determines which frame of a movie to display. Scene time applies only to animations whose usesSceneTimeBase property is true, including those loaded from a scene source using the playUsingSceneTimeBase option.

Use this property, together with the above animation options, when you want to directly control (or allow the user to directly control) the playback of animations. For example, if you’re building an authoring tool for 3D assets, you might bind this property’s value to a slider control for scrubbing through playback of animations in a scene file.

## See Also

### Managing Scene Animation Timing

var isPlaying: Bool

A Boolean value that determines whether the scene is playing.

**Required**

var loops: Bool

A Boolean value that determines whether SceneKit restarts the scene time after all animations in the scene have played.

**Required**

