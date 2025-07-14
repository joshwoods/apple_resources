

- RealityKit
- Views and attachments
- Postprocessing effects
-  Applying core image filters as a postprocess effect 

Article

# Applying core image filters as a postprocess effect

Create special rendering effects for your RealityKit scenes using Core Image.

## Overview

In iOS 15 and later, and macOS 12 and later, you can apply postprocess effects to a RealityKit scene after RealityKit renders it, but before RealityKit displays it. If you register a postprocess callback function, RealityKit passes that function the complete, rendered frame so you can modify it before the viewer sees it. You can use any image processing or drawing APIs on the rendered frame but, as a practical matter, only APIs that execute on the GPU are fast enough to use every frame and maintain a good framerate.

One option for implementing postprocess effects is to apply Core Image filters to the rendered frame. Core Image provides a wide variety of filters that implement different image effects and execute on the GPU, making them a good choice for postprocessing effects.

You may also wish to look at the Metal Performance Shaders framework as an alternative. The Metal Performance Shaders framework offers a smaller set of image filters than Core Image, but they operate directly on Metal textures and can use an existing MTLComputeCommandEncoder. That means they take less code to implement and are more efficient than Core Image filters because you don’t have to convert the MTLTexture containing the rendered frame into a CIImage before applying the filter.

For information on using Image Filters from the Metal Performance Shaders framework, see Using Metal performance shaders to create custom postprocess effects. If neither Core Image nor the Metal Performance Shaders framework provide the effect you need, you can also write custom compute functions to implement postprocess effects. For more information about postprocessing with compute functions, see Implementing postprocess effects using Metal compute functions.

### Set up the core image context

In order to apply a CIFilter, you need to create a CIContext during app launch and store it in a property so it’s available to your postprocess callback. You can use a single Core Image context regardless of the number or types of filters you use. The prepareWithDevice render callback is a good place to create your context and do other setup work. RealityKit calls the prepareWithDevice function once, after does its own setup, but before it renders the next frame.

If you set the callback at launch, RealityKit calls it before it draws the first frame. This is a good place to do setup tasks, especially processor-intensive or time-consuming tasks, such as loading images, or tasks that require access to the MTLDevice, which RealityKit passes to the callback function.

To create a prepareWithDevice callback, write a function that takes a single MTLDevice parameter and has no return value. In that function, create and store a CIContext and do any other necessary setup tasks, such as loading textures needed by the filter.

```
func setupCoreImage(device: MTLDevice) {
    // Create a CIContext and store it in a property.
    ciContext = CIContext(mtlDevice: device)

    // Do other expensive tasks, like loading images, here.
}
```

Next, register the function as a callback by assigning it to the prepareWithDevice property of the view’s renderCallbacks property.

```
arView.renderCallbacks.prepareWithDevice = setupCoreImage
```

To make sure your setup code fires before rendering begins, assign the prepareWithDevice callback in code that executes during app startup, such as in your main view controller’s viewWillAppear(_:) method or the main SwiftUI view’s makeUIView(context:) method. RealityKit does call a prepareWithDevice callback if it’s registered after RealityKit starts rendering the scene, but doing setup tasks after rendering has started can cause a rendering hitch.

### Check the output texture pixel format

Some device GPUs require that the output texture be in a specific pixel format. If the device your code is running on doesn’t support MTLGPUFamily.apple2, convert the output texture to the MTLPixelFormat.bgra8Unorm before using it. For more information, see Checking the pixel format of a postprocess effect’s output texture.

### Create a postprocess callback function

Next, create the render callback function. Once you register it, RealityKit calls it every frame before displaying the rendered scene. In the callback, configure your CIFilter, convert the source color texture — which contains the frame buffer — into a CIImage, and set it as the filter’s image input. Then, create a CIRenderDestination, and render the filter to it.

```
func postProcessWithCoreImage(context: ARView.PostProcessContext) {

    // Create and configure the Core Image filter.
    let filter = CIFilter.falseColor()
    filter.color0 = CIColor.blue
    filter.color1 = CIColor.yellow

    // Convert the frame buffer from a Metal texture to a CIImage, and 
    // set the CIImage as the filter's input image.
    guard let input = CIImage(mtlTexture: context.sourceColorTexture) else {
        fatalError("Unable to create a CIImage from sourceColorTexture.")
    }
    filter.setValue(input, forKey: kCIInputImageKey)

    // Get a reference to the filter's output image.
    guard let output = filter.outputImage else {
        fatalError("Error applying filter.")
    }

    // Create a render destination and render the filter to the context's command buffer.
    let destination = CIRenderDestination(mtlTexture: context.compatibleTargetTexture,
                                          commandBuffer: context.commandBuffer)
    destination.isFlipped = false
    _ = try? self.ciContext.startTask(toRender: output, to: destination)
}
```

Note

The `compatibleTargetTexture` property referenced above is a derived property based on targetColorTexture. It ensures that the output texture uses the appropriate pixel format for the current device. For more information, see Checking the pixel format of a postprocess effect’s output texture.

### Register the callback function

To apply the effect, register the function as the postProcess render callback for the ARView.

```
arView.renderCallbacks.postProcess = postProcessWithCoreImage
```

Note

For more information on using Core Image to create postprocess effects, see the Implementing Special Rendering Effects with RealityKit Postprocessing sample code, which demonstrates multiple postprocess techniques, including Core Image.

