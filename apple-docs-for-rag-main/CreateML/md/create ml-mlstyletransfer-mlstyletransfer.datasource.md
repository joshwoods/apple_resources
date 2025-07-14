

- Create ML
- MLStyleTransfer
-  MLStyleTransfer.DataSource 

Enumeration

# MLStyleTransfer.DataSource

A data source for a style transfer model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
enum DataSource
```

## Topics

### Creating a data source

case images(styleImage: URL, contentDirectory: URL, processingOption: VNImageCropAndScaleOption?)

The locations of a style-image file and content-image directory in the file system.

### Stylizing images

func processImages(textelDensity: Int, styleImageDestination: URL?, contentImagesDestination: URL?) throws -> (processedStyleImage: URL, processedContentImages: URL)

Converts the content images to square images and saves them to a destination directory.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting types

struct ModelParameters

Parameters that affect the training process of a style transfer model.

