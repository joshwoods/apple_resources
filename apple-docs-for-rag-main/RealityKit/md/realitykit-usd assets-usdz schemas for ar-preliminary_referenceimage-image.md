

- RealityKit
- USD Assets
- USDZ schemas for AR
- Preliminary_ReferenceImage
-  image 

Article

# image

An image file for which the runtime should search.

## Overview

Assign this property a path to a PNG or JPEG file.

### Declaration

```
uniform asset image
```

### Define a reference image

The following Preliminary_ReferenceImage assigns this property a file named `image.png`.

```
def Preliminary_ReferenceImage "ImageReference"
{
    uniform asset image = @image.png@
    ...
}
```

## See Also

### Properties

physicalWidth

An image’s width in centimeters.

