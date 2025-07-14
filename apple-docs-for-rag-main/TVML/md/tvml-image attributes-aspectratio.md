

- TVML
- Image Attributes
-  aspectRatio 

Article

# aspectRatio

Specifies the aspect ratio of an image.

## Overview

Use the `aspectRatio` attribute when setting the image’s `contentsMode` to provide TVMLKit with the context needed to determine how to fit the source image in the view port.

The attribute’s value should correlate with the aspect ratio of the source image. The value is a `double` derived by dividing the width of the aspect ratio by the height. Here’s an example that demonstrates the `aspectRatio` attribute used to specify a source image with a 3 to 2 width to height ratio.

```

```

### Elements that Use aspectRatio

- contentsMode

## See Also

### Image Size

height

Specifies the maximum height for an image.

width

Specifies the maximum width for an image element.

