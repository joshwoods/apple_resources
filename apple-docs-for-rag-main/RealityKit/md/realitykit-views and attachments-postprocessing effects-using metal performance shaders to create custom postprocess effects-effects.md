

- RealityKit
- Views and attachments
- Postprocessing effects
-  Using Metal performance shaders to create custom postprocess effects 

Article

# Using Metal performance shaders to create custom postprocess effects

Leverage the Metal Performance Shaders framework to create special rendering effects for your RealityKit scenes.

## Overview

In iOS 15 and later, and macOS 12 and later, you can apply postprocess effects to a RealityKit scene after RealityKit renders it, but before RealityKit displays it. If you register a postprocess callback function, RealityKit passes that function the complete, rendered frame so you can modify it before the viewer sees it. You can use any image processing or drawing APIs on the rendered frame but, as a practical matter, only APIs that execute on the GPU are fast enough to use every frame and maintain a good framerate.

One way to implement postprocess effects is to apply filters from the Metal Performance Shaders framework to the rendered scene. You can use apply these filters to an image without writing any custom shader code. Because these filters run on the GPU and operate directly on Metal textures, they’re a good choice for postprocessing effects.

If the Metal Performance Shaders framework doesn’t provide an image filter that meets your needs, you can also use Core Image to postprocess frames. Core Image provides a greater selection of image filters, which also run on the GPU, but Core Image requires you to convert the rendered frame into a CIImage. For more information, see Applying core image filters as a postprocess effect.

If neither the Metal Performance Shaders framework nor Core Image provide the effect you need, you can also write custom compute functions to implement postprocess effects. For more information, see Implementing postprocess effects using Metal compute functions.

### Check the output texture pixel format

Some device GPUs require that the output texture be in a specific pixel format. If the device your code is running on doesn’t support MTLGPUFamily.apple2, convert the output texture to MTLPixelFormat.bgra8Unorm before using it. For more information, see Checking the pixel format of a postprocess effect’s output texture.

### Create a callback function

To create postprocess effects using image filters from the Metal Performance Shaders framework, create a Swift function that takes a single ARView.PostProcessContext parameter. In that method, create and configure an instance of the filter that you want to apply using the device property from the context. Once you’ve created an instance of the shader, call its encode method, passing the command buffer, source color texture, and output texture from the context.

```
    func postEffectMPSGaussianBlur(context: ARView.PostProcessContext) {
        let gaussianBlur = MPSImageGaussianBlur(device: context.device, sigma: 4)
        gaussianBlur.encode(commandBuffer: context.commandBuffer,
                            sourceTexture: context.sourceColorTexture,
                            destinationTexture: context.compatibleTargetTexture)
```

Note

The `compatibleTargetTexture` property referenced above is a derived property based on targetColorTexture. It ensures that the output texture uses the appropriate pixel format for the current device. For more information, see Checking the pixel format of a postprocess effect’s output texture.

### Register the callback function

To apply the effect, register the function as the postProcess render callback for the ARView.

```
arView.renderCallbacks.postProcess = postEffectMPSGaussianBlur
```

Note

For more information on using Metal Performance Shader framework image filters to create postprocess effects, see the Implementing Special Rendering Effects with RealityKit Postprocessing sample code project.

## See Also

### Metal effects

Implementing Special Rendering Effects with RealityKit Postprocessing

Implement a variety of postprocessing techniques to alter RealityKit rendering.

Checking the pixel format of a postprocess effect’s output texture

Make sure your postprocess effect works on all devices.

Passing Structured Data to a Metal Compute Function

Send nontexture data from Swift to your Metal shaders using a shared header file.

Implementing postprocess effects using Metal compute functions

Create custom shaders to implement postprocess effects.

