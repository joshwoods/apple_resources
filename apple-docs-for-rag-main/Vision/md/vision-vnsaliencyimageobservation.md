

- Vision
-  VNSaliencyImageObservation 

Class

# VNSaliencyImageObservation

An observation that contains a grayscale heat map of important areas across an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNSaliencyImageObservation
```

## Overview

The heat map is a CVPixelBuffer in a one-component floating-point pixel format. Its dimensions are 64 x 64 when fetched in real time, or 68 x 68 when requested in its deferred form.

## Topics

### Locating Salient Regions

var salientObjects: [VNRectangleObservation]?

A collection of objects describing the distinct areas of the saliency heat map.

## Relationships

### Inherits From

- VNPixelBufferObservation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

## See Also

### Saliency analysis

Cropping Images Using Saliency

Isolate regions in an image that are most likely to draw people’s attention.

Highlighting Areas of Interest in an Image Using Saliency

Quantify and visualize where people are likely to look in an image.

class VNGenerateAttentionBasedSaliencyImageRequest

An object that produces a heat map that identifies the parts of an image most likely to draw attention.

class VNGenerateObjectnessBasedSaliencyImageRequest

A request that generates a heat map that identifies the parts of an image most likely to represent objects.

