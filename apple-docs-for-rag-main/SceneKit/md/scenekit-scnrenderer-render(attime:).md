

- SceneKit
- SCNRenderer
-  render(atTime:) 

Instance Method

# render(atTime:)

Renders the scene’s contents at the specified system time in the renderer’s OpenGL context.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOS

``` source
func render(atTime time: CFTimeInterval)
```

## Parameters 

`time`  

The timestamp, in seconds, at which to render the scene.

## Discussion

This method can be used only with an SCNRenderer object created with the SCNRenderer initializer. Call this method to tell SceneKit to draw the renderer’s scene into the OpenGL context you created the renderer with.

When you call this method, SceneKit updates its hierarchy of presentation nodes based on the specified timestamp, and then draws the scene.

Note

By default, the playback timing of actions and animations in a scene is based on the system time, not the scene time. Before using this method to control the playback of animations, set the usesSceneTimeBase property of each animation to true, or specify the playUsingSceneTimeBase option when loading a scene file that contains animations.

## See Also

### Rendering a Scene Using OpenGL

func render()

Renders the scene’s contents in the renderer’s OpenGL context.

Deprecated

