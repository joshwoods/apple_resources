

- TVML
- Image Attributes
-  mode 

Article

# mode

Specifies how an image is displayed.

## Overview

Use the `mode` attribute to define how an image is displayed in the `oneupTemplate` and `showcaseTemplate` elements. The `showcaseTemplate` element can only use the `showcase oneup` attribute value. The `oneupTemplate` can only use the `oneup caption` attribute value. Clicking an image alternates between the selected modes. Here’s an example that displays images in `showcaseTemplate` in `showcase` mode:

```

            Scenes

                    Slideshow

                    Screensaver

                    Scene 1

                    Scene 2

```

### Values for mode

`showcase oneup`  
Image alternates between the actual image size and a fullscreen image.

`oneup caption`  
Image alternates between a fullscreen image with or without a caption below the image.

### Elements that Use mode

- oneupTemplate

- showcaseTemplate

## See Also

### Image Display

aspectFill

Stretches an image to fill the containing bounding box.

contentsMode

Specifies how an image is expanded to fill its containing element.

opaque

Indicates whether an image has a transparent background.

type

Specifies how a badge is drawn.

value

Specifies the value used for a fillable element.

