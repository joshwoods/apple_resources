

- SpriteKit
- SK3DNode
-  sceneTime 

Instance Property

# sceneTime

The current scene time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**watchOS**

``` source
var sceneTime: TimeInterval { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var sceneTime: TimeInterval { get set }
```

## Discussion

This timestamp determines the behavior of running animations, similar to how the playhead time in a video player application determines which frame of a movie to display. It applies only to animations whose usesSceneTimeBase property is true, including those loaded from a scene source using the playUsingSceneTimeBase option.

Use this property together with the above animation options when you want to directly control (or allow the user to directly control) the playback of animations.

## See Also

### Animating a 3D Node’s Content in Scene Kit

var isPlaying: Bool

A Boolean value that determines whether the scene is playing.

var loops: Bool

A Boolean value that determines whether Scene Kit restarts the scene time after all animations in the scene have played.

