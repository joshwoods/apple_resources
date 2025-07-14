

- RealityKit
- ARView
- ARView.RenderCallbacks
-  postProcess 

Instance Property

# postProcess

A callback function for implementing postprocess effects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var postProcess: ((ARView.PostProcessContext) -> Void)?
```

## Mentioned in 

Implementing postprocess effects using Metal compute functions

Applying core image filters as a postprocess effect

Using Metal performance shaders to create custom postprocess effects

## Discussion

Assign a function or closure to this property to implement postprocessing effects for a RealityKit scene. If this value is non-`nil`, RealityKit calls the assigned function or closure once every frame before it displays the scene. If you register a postprocess render callback, the callback function needs to encode the modified frame buffer to the context’s targetColorTexture, or nothing renders.

A postprocess callback looks like this:

```
func myPostProcessCallback(context:ARView.PostProcessContext) {
   // Handle postprocessing here.
}
```

To register the function so RealityKit begins calling it, assign it to the postProcess property of the view’s renderCallbacks property.

```
arView.renderCallbacks.postProcess = myPostProcessCallback
```

To stop RealityKit from calling your function, assign `nil`:

```
arView.renderCallbacks.postProcess = nil
```

If your app turns postprocessing on and off frequently, another option for disabling postprocess effects is to keep your callback registered, but use an MTLBlitCommandEncoder to encode the unmodified frame directly to the output texture whenever postprocess effects aren’t active.

```
func myPostProcessCallback(context:ARView.PostProcessContext) {
    if (usePostProcessEffects) {
        handlePostProcessing(context: ARView.PostProcessContext)
        return
    }

    // If postprocess effects are disabled, copy sourceColorTexture
    // directly to targetColorTexture.
    let blitEncoder = context.commandBuffer.makeBlitCommandEncoder()
    blitEncoder?.copy(from: context.sourceColorTexture, to: context.targetColorTexture)
    blitEncoder?.endEncoding()
}
```

## See Also

### Register callback closures

var prepareWithDevice: ((any MTLDevice) -> Void)?

A callback function for doing initial setup work.

