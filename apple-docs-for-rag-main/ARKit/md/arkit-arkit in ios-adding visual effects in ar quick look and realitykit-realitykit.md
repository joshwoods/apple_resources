

- ARKit
- ARKit in iOS
-  Adding Visual Effects in AR Quick Look and RealityKit 

Article

# Adding Visual Effects in AR Quick Look and RealityKit

Balance the appearance and performance of your AR experiences with modeling strategies.

## Overview

AR Quick Look supports modeling features you can use to present your app’s virtual content at its most vivid and compelling. Make sure to optimize the performance of your AR experience by managing and testing the features you incorporate.

AR Quick Look uses RealityKit to display AR experiences, and you can design your models to take advantage of features in RealityKit available on iOS 13 and later. Roughness, for instance, is a property that affects how light diffuses on matte surfaces. RealityKit implements roughness using a multiscattering algorithm, enhancing the texture and realism of virtual content. Additionally, you can use the clearcoat option to add a glossy shine to your virtual content.

### Add Gloss to Your 3D Content with Clearcoat

You can add shine and highlights to the models in your AR experience with the clearcoat option.

RealityKit renders clearcoat by adding a second specular lobe. To enable a clearcoat layer on your app’s virtual content, use the following inputs when designing your model:

`clearcoat`  
A scalar float normalized between 0 and 1 that indicates the intensity of the clearcoat specular lobe.

`clearcoatRoughness`  
A float normalized between 0 and 1 that indicates the perceived roughness of the clearcoat surface.

The following figure shows the `clearcoat` parameter varying between 0 and 1 vertically, and `clearcoatRoughness` varying between 0 and 1 horizontally, with (0, 0) at the bottom left.

### Design for Lighting and Reflection Accuracy

RealityKit’s multiscattering roughness affects how light reflects from––or diffuses on––the surface of models with a matte finish. By displaying virtual content using RealityKit, AR Quick Look realistically honors the roughness, metallic, and specular components of a model. Configure your 3D assets’ roughness, metallic, and specular inputs to create the right blend of reflection and diffusion.

The roughness component controls the texture of a surface. A roughness value of 0 (smooth) results in a mirror reflection, while a roughness value of 1 (rough) diffuses light to create a surface without shine. The following figure shows the `roughness` parameter varying between 0 and 1, with 0 on the left.

The metallic component defines whether your model appears dielectric (0) or metallic (1). The following figure shows the `metallic` parameter varying from 0-1, with 0 on the left.

For dielectrics, the specular component enables you to control the reflectiveness of a surface, ranging from 0 (nonreflective) to 1 (fully reflective). The following figure shows a roughness with the `specular` parameter varying from 0-1, with 0 on the left.

Note

Environment lighting in AR Quick Look supports multiple models in iOS 13. To ensure your virtual content displays with the most realistic reflections in your app, check the iOS version at runtime and load multiple models only in iOS 13.

### Optimize Model Geometry and Transparency

While utilizing features to present virtual content effectively, take steps to keep the AR experience responsive. Because each model mesh results in a draw call, for best results, limit the number of meshes in a USDZ file to around 50. To reduce draw calls while maintaining the same amount of geometry, merge objects that share a material. However, be aware that merging may not afford performance gains in situations where the result prevents the renderer from culling.

The cost of projective and raytraced shadows depends on the complexity of your model’s geometry. To enhance performance and prevent excessive memory use relating to lighting, keep the polygon count of your 3D asset’s geometry below 100,000 polygons.

Transparency in models increases the number of times the fragment shader is run per pixel, which is expensive when the user views your model straight on or in full screen. To improve performance by reducing the time your app spends shading pixels, use transparency sparingly when authoring your app’s virtual content.

### Control Texture Memory

For best results, size your textures to 1024 x 1024 pixels or less, and don’t surpass a size of 2048 x 2048 pixels. If you have multiple small textures, combine them into one larger texture using texture coordinates to specify their location. To ensure your textures fit into memory as required for AR Quick Look to display your model, cap your total number of textures at six.

If you observe any resolution discrepancies at runtime, switch to testing on a device with more memory and check for any differences. AR Quick Look automatically generates mipmaps for your model’s textures. AR Quick Look also scales down your texture at runtime if needed to keep its memory use under a certain budget depending on the device.

### Test Features on Various Devices

When developing your model for optimal performance, begin with a conservative configuration to ensure AR Quick Look supports your model on earlier iOS devices (iPhone 6s, and first-generation iPad Pro). By starting on the earliest devices that support AR Quick Look, you avoid having to prune back your virtual content’s features during the testing phase.

## See Also

### AR Quick Look

Previewing a Model with AR Quick Look

Display a model or scene that the user can move, scale, and share with others.

Adding an Apple Pay Button or a Custom Action in AR Quick Look

Provide a banner that users can tap to make a purchase or perform a custom action in an AR experience.

class ARQuickLookPreviewItem

An object for customizing the AR Quick Look experience.

USDZ schemas for AR

Add augmented reality functionality to your 3D content using USDZ schemas.

Specifying a lighting environment in AR Quick Look

Add metadata to your USDZ file to specify its lighting characteristics.

