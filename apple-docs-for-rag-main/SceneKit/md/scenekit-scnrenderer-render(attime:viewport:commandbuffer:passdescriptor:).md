

- SceneKit
- SCNRenderer
-  render(atTime:viewport:commandBuffer:passDescriptor:) 

Instance Method

# render(atTime:viewport:commandBuffer:passDescriptor:)

Renders the scene’s contents at the specified system time in the specified Metal command buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func render(
    atTime time: CFTimeInterval,
    viewport: CGRect,
    commandBuffer: any MTLCommandBuffer,
    passDescriptor renderPassDescriptor: MTLRenderPassDescriptor
)
```

## Parameters 

`time`  

The timestamp, in seconds, at which to render the scene.

`viewport`  

The pixel dimensions in which to render.

`commandBuffer`  

The Metal command buffer in which SceneKit should schedule rendering commands.

`renderPassDescriptor`  

The Metal render pass descriptor describing the rendering target.

## Discussion

This method can be used only with an SCNRenderer object created with the SCNRenderer initializer. Call this method to tell SceneKit to draw the renderer’s scene into the render target described by the `renderPassDescriptor` parameter, by encoding render commands into the `commandBuffer` parameter.

When you call this method, SceneKit updates its hierarchy of presentation nodes based on the specified timestamp, and then draws the scene using the specified Metal objects.

Note

By default, the playback timing of actions and animations in a scene is based on the system time, not the scene time. Before using this method to control the playback of animations, set the usesSceneTimeBase property of each animation to true, or specify the playUsingSceneTimeBase option when loading a scene file that contains animations.

