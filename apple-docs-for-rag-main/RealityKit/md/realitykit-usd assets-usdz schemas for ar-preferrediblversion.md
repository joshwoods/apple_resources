

- RealityKit
- USD Assets
- USDZ schemas for AR
-  preferredIblVersion 

Article

# preferredIblVersion

Metadata that determines the lighting environment of virtual content.

## Overview

This metadata selects one of two predefined options for the scene’s image-based lighting (IBL). AR Quick Look in iOS 16 and later observes this property to enhance the brightness, contrast, and visual definition of a scene’s virtual content.

A value of `1` indicates the classic lighting environment, and a value of `2` indicates the new lighting environment.

If you omit the preferredIblVersion metadata or give it a value of `0`, the system checks the asset’s creation timestamp. A timestamp of July 1, 2022, or later results in the new lighting environment; otherwise, the scene features classic lighting for backward compatibility. The system checks the timestamp of the `.usd` asset within the `.usdz` archive, not the archive’s file creation date.

### Declaration

```
int preferredIblVersion = 0
```

### Select the scene’s image-based lighting

The following `.usda` definition chooses the new lighting environment:

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

Tip

RealityKit doesn’t observe the preferredIblVersion metadata, but you configure the same lighting environment manually. See Specifying a lighting environment in AR Quick Look for more information about matching AR Quick Look’s lighting environment in RealityKit apps.

## See Also

### Scenes and lighting

Specifying a lighting environment in AR Quick Look

Add metadata to your USDZ file to specify its lighting characteristics.

sceneLibrary

Metadata that partitions an asset into scene-based units.

