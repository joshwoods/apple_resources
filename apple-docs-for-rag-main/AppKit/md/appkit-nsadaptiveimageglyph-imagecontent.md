

- AppKit
- NSAdaptiveImageGlyph
-  imageContent 

Instance Property

# imageContent

The raw data for the image.

macOS 15.0+

``` source
var imageContent: Data { get }
```

## Discussion

This property contains the image data, the unique identifier for the image, the image description, and additional metadata. When saving your content to disk, save the data for any adaptive images with the rest of your content. If you need to specify a type for the image data, use the value in the contentType property.

