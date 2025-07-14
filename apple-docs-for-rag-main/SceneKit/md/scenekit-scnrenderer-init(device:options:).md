

- SceneKit
- SCNRenderer
-  init(device:options:) 

Initializer

# init(device:options:)

Creates a renderer with the specified Metal device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    device: (any MTLDevice)?,
    options: [AnyHashable : Any]? = nil
)
```

## Parameters 

`device`  

A Metal device.

`options`  

An optional dictionary for future extensions.

## Return Value

A new renderer object.

## Discussion

Use this initializer to create a SceneKit renderer that draws into the rendering targets your app already uses to draw other content. For the `device` parameter, pass the MTLDevice object your app uses for drawing. Then, to tell SceneKit to render your content, call the SCNRenderer method, providing a command buffer and render pass descriptor for SceneKit to use in its rendering.

## See Also

### Creating a Renderer

convenience init(context: EAGLContext?, options: [AnyHashable : Any]?)

Creates a renderer with the specified OpenGL context.

