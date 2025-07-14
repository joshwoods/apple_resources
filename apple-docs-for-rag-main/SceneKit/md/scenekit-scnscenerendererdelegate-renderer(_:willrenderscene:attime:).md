

- SceneKit
- SCNSceneRendererDelegate
-  renderer(\_:willRenderScene:atTime:) 

Instance Method

# renderer(\_:willRenderScene:atTime:)

Tells the delegate that the renderer has cleared the viewport and is about to render the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
optional func renderer(
    _ renderer: any SCNSceneRenderer,
    willRenderScene scene: SCNScene,
    atTime time: TimeInterval
)
```

## Parameters 

`renderer`  

The SceneKit object responsible for rendering the scene. Examine this object’s context property if you need to reference the OpenGL context that your custom rendering code draws into.

`scene`  

The `SCNScene` object to be rendered.

`time`  

The current system time, in seconds. If your custom rendering involves animation, use this parameter to compute your own animation state.

## Discussion

Implement this method to perform custom drawing before SceneKit renders a scene—for example, to draw backdrop content underneath SceneKit content. You should only execute Metal or OpenGL drawing commands (and any setup required to perform them) in this method—the results of modifying SceneKit objects during this method are undefined.

- To render using Metal, use the `renderer` parameter to retrieve the scene renderer’s currentRenderCommandEncoder object and encode your own drawing commands. If you need to reference other Metal state, see the properties listed in SCNSceneRenderer.

- To render using OpenGL, simply call the relevant OpenGL drawing commands—SceneKit automatically makes its OpenGL context the current context before calling this method. If you need to reference the OpenGL context being rendered into, examine the context property of the `renderer` parameter.

You must draw using the appropriate graphics technology for the view currently being rendered. Use the renderingAPI property of the `renderer` object to determine whether Metal or OpenGL is in use.

## See Also

### Rendering Custom Scene Content

func renderer(any SCNSceneRenderer, didRenderScene: SCNScene, atTime: TimeInterval)

Tells the delegate that the renderer has rendered the scene.

