

- RealityKit
- Views and attachments
- Postprocessing effects
-  Checking the pixel format of a postprocess effect’s output texture 

Article

# Checking the pixel format of a postprocess effect’s output texture

Make sure your postprocess effect works on all devices.

## Overview

Some device GPUs require that the output texture for postprocess effects be in a specific format. If the current device doesn’t support MTLGPUFamily.apple2, convert the output texture to MTLPixelFormat.bgra8Unorm before encoding the processed framebuffer to it. An easy way to do that, is to add a derived property to ARView.PostProcessContext using an extension:

```
extension RealityKit.ARView.PostProcessContext {
    // Returns the output texture, ensuring that the pixel format is 
    // appropriate for the current device's GPU.
    var compatibleTargetTexture: MTLTexture! {
        if self.device.supportsFamily(.apple2) {
            return targetColorTexture
        } else {
            return targetColorTexture.makeTextureView(pixelFormat: .bgra8Unorm)!
        }
    }
}
```

If you use this derived property instead of targetColorTexture when encoding the results of a postprocess effect, it ensures the effect works on all devices.

## See Also

### Metal effects

Using Metal performance shaders to create custom postprocess effects

Leverage the Metal Performance Shaders framework to create special rendering effects for your RealityKit scenes.

Implementing Special Rendering Effects with RealityKit Postprocessing

Implement a variety of postprocessing techniques to alter RealityKit rendering.

Passing Structured Data to a Metal Compute Function

Send nontexture data from Swift to your Metal shaders using a shared header file.

Implementing postprocess effects using Metal compute functions

Create custom shaders to implement postprocess effects.

