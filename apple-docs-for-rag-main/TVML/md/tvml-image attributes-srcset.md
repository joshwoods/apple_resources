

- TVML
- Image Attributes
-  srcset 

Article

# srcset

Specifies multiple URLs for an image.

## Overview

Use the `srcset` attribute to specify different URLs for an image depending on the situation. The URL can point to an image on a server or to the resource scheme in your app. For a list of resource images provide by Apple, see the Resource Icons section of TVML. Here’s an example that displays a different chevron image depending whether the current language is a left-to-right or right-to-left language.

```

```

`srcset` is also used to specify images for 4K devices. Non-4K images are indicated with a 1x, while 4K images are indicated with a 2x. Here’s an example showing how to specify different images for 4K and non-4K devies.

```

```

Note

When this attribute loads an image using an HTTP URL, you must add `height` and `width` attributes to the element.

### Values for srcset

String  
The URL pointing to the location of the image file.

### Elements that Use srcset

- badge

- decorationImage

- fullscreenImg

- heroImg

- img

## See Also

### Image Retrieval

src

Specifies the URL for an image.

