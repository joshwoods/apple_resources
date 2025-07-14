

- RealityKit
- USD Assets
- USDZ schemas for AR
- Preliminary_ReferenceImage
-  physicalWidth 

Article

# physicalWidth

An image’s width in centimeters.

## Overview

This property informs the runtime how wide the image is in the physical environment. The runtime calculates the height based on the image’s aspect ratio.

Because this property describes a real-world width, the prim’s transform hierarchy doesn’t modify this property’s value.

### Declaration

```
uniform double physicalWidth
```

### Define a reference image’s width

To recognize an image in the real world, the runtime requires a prim to specify how wide the image is in the physical environment.

```
def Preliminary_ReferenceImage "ImageReference"
{
    uniform double physicalWidth = 12
    ...
}
```

## See Also

### Properties

image

An image file for which the runtime should search.

