

- UIKit
- UIImageReader
-  UIImageReader.Configuration 

Structure

# UIImageReader.Configuration

The properties that a reader uses to decode images.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOSwatchOS 10.0+

``` source
struct Configuration
```

## Topics

### Creating the configuration

init()

Creates a new instance of the image reader configuration.

### Configuration properties

var prefersHighDynamicRange: Bool

A Boolean value that indicates whether the image reader should decode the image as HDR when the type is capable of decoding in either SDR or HDR.

var preparesImagesForDisplay: Bool

A Boolean value that indicates whether the image reader prepares the image for display.

var preferredThumbnailSize: CGSize

The thumbnail size in pixels that the image reader makes the image.

var pixelsPerInch: Double

The integral scale that the image reader applies to the image.

## Relationships

### Conforms To

- Equatable

