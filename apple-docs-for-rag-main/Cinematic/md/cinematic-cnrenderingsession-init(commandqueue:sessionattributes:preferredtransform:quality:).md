

- Cinematic
- CNRenderingSession
-  init(commandQueue:sessionAttributes:preferredTransform:quality:) 

Initializer

# init(commandQueue:sessionAttributes:preferredTransform:quality:)

Intializes an object for a rendering session.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
init(
    commandQueue: any MTLCommandQueue,
    sessionAttributes: CNRenderingSession.Attributes,
    preferredTransform: CGAffineTransform,
    quality: CNRenderingQuality
)
```

## Parameters 

`commandQueue`  

The command queue of a metal device that creates the command buffer.

`sessionAttributes`  

Rendering session attributes loaded from a cinematic asset.

`preferredTransform`  

The preferred transform of the rendered image for display purposes. Always the identity transform or a multiple of a 90º rotation with no scaling.

`quality`  

The quality of rendering desired for a session. Quality levels include thumbnail, preview, and three export quality levels. You can create more than one session for the same video with different quality levels.

