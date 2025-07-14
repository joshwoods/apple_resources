

- TVML
- Image Attributes
-  contentsMode 

Article

# contentsMode

Specifies how an image is expanded to fill its containing element.

## Overview

Use the `contentsMode` attribute to specify how the image is scaled within its bounding box. Here’s an example that demonstrates the `contentsMode` attribute in a `stackTemplate`:

```

            contentsMode

                        aspectFit

                        aspectFitBB

                        aspectFill

```

Important

When using the `aspectFit` value, you must also include the aspectRatio attribute for the content to scale appropriately.

### Values

aspectFit  
The image scales to fit in the bounding box using fixed aspect ratio. The output bounding box has the same size as the scaled image, leaving no remaining area. The output bounding box may be smaller than its specified size.

aspectFitBB  
The image scales to fit in the bounding box using fixed aspect ratio. The output bounding box keeps its specified size. Any unfilled area of the bounding box is white.

aspectFill  
The image scales to fill in the bounding box using fixed aspect ratio. Portions of the image may be clipped.

### Elements That Use contentsMode

- img

## See Also

### Image Display

aspectFill

Stretches an image to fill the containing bounding box.

opaque

Indicates whether an image has a transparent background.

mode

Specifies how an image is displayed.

type

Specifies how a badge is drawn.

value

Specifies the value used for a fillable element.

