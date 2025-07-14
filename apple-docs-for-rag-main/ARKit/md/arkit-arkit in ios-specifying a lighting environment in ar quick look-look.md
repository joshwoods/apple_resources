

- ARKit
- ARKit in iOS
-  Specifying a lighting environment in AR Quick Look 

Article

# Specifying a lighting environment in AR Quick Look

Add metadata to your USDZ file to specify its lighting characteristics.

## Overview

AR Quick Look in iOS 16 and later enhances lighting to deliver more brightness, contrast, and visual definition for your scene’s virtual content.

You can set an asset’s lighting environment, or *image-based lighting* (IBL), by adding the preferredIblVersion metadata to the file’s `.usda` textual definition, or by generating the asset with Apple-provided tools.

### Set the lighting metadata

To define the lighting environment in the asset’s `.usda` textual format using a tool like USD Toolset, add the following metadata:

```
// asset.usda
#usda 1.0
(
    customLayerData = {
        dictionary Apple = {
            int preferredIblVersion = 2
        }
    }
)
```

A value of `1` indicates the classic lighting environment, and a value of `2` indicates the new lighting environment.

If you omit the preferredIblVersion metadata or give it a value of `0`, the system checks the asset’s creation timestamp. A timestamp of July 1, 2022, or later results in the new lighting environment; otherwise, the scene features classic lighting for backward compatibility. The system checks the timestamp of the `.usd` asset within the `.usdz` archive, not the archive’s file creation date.

### Set the lighting environment with Apple-provided tools

With Reality Converter, you can choose a lighting preferrence for your 3D asset by previewing the available options one after the other. By default, Reality Converter previews an imported 3D asset with `preferrediblversion` = `2`. You can select the Use Classic Lighting option to set `preferrediblversion` to `1` in the file.

Alternatively, you can use `usdzconvert` in the Apple USDZ Tools suite to output from another file format. Pass an integer value between `0` and `2` for the `--preferrediblversion` argument to add this metadata in the file, as the following example shows:

```
usdzconvert fireHydrant.obj --useObjMtl --preferrediblversion 2 
```

### Match AR Quick Look lighting in third-party apps and tools

To design your content in a third-party digital content creation tool (DCC) under the same lighting conditions as AR Quick Look’s lighting environment, configure the tool to use one of the following `.exr` files. Alternatively, you can apply an `.exr` file in your third-party app, such as one that renders with RealityKit, to accommodate the new lighting environment in your app’s runtime experience.

- The studio_lighting_objectmode_v002.exr file provides reflections that match AR Quick Look’s studio object mode. This IBL is appropriate for asset creation in a third-party DCC. Consult the DCC documentation about enabling custom image-based lighting in the tool.

- The studio_lighting_armode_v002.exr file provides enhanced highlights according to AR Quick Look’s new lighting environment in AR mode. This IBL is appropriate for use in your AR app as a combination with an environment texture that composes captures of the user’s environment. Together, the combination enhances reflections on your app’s virtual content that feature the particular tints and hues of the real world.

Tip

For apps that render virtual content using RealityKit, set up a skybox with the AR mode IBL to use the new lighting environment. Although AR Quick Look observes the `preferrediblversion` metadata, RealityKit doesn’t. See EnvironmentResource for more information about defining image-based lighting in RealityKit.

## See Also

### AR Quick Look

Previewing a Model with AR Quick Look

Display a model or scene that the user can move, scale, and share with others.

Adding Visual Effects in AR Quick Look and RealityKit

Balance the appearance and performance of your AR experiences with modeling strategies.

Adding an Apple Pay Button or a Custom Action in AR Quick Look

Provide a banner that users can tap to make a purchase or perform a custom action in an AR experience.

class ARQuickLookPreviewItem

An object for customizing the AR Quick Look experience.

USDZ schemas for AR

Add augmented reality functionality to your 3D content using USDZ schemas.

