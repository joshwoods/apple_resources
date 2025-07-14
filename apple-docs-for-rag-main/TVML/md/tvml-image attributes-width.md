

- TVML
- Image Attributes
-  width 

Article

# width

Specifies the maximum width for an image element.

## Overview

The image is shrunk to fit the bounding box if the image is bigger than the size specified for the `width` attribute. You must declare either a `width` style or attribute for an image. Declaring a style overwrites an attribute declaration. Here’s an example that sets the width for an image to 200 points.

```

```

### Values for width

Integer  
The width of the element, in points.

### Elements that Use width

- decorationLabel

- fullscreenImg

- heroImg

- img

Note

When an image is a child of a `lockup` element, the longest dimension of the image must be 70 points longer than the corresponding bounding box dimension.

## See Also

### Image Size

height

Specifies the maximum height for an image.

aspectRatio

Specifies the aspect ratio of an image.

