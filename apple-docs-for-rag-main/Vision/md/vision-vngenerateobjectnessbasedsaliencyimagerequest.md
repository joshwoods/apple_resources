

- Vision
-  VNGenerateObjectnessBasedSaliencyImageRequest 

Class

# VNGenerateObjectnessBasedSaliencyImageRequest

A request that generates a heat map that identifies the parts of an image most likely to represent objects.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNGenerateObjectnessBasedSaliencyImageRequest
```

## Overview

The resulting observation, VNSaliencyImageObservation, encodes this data as a heat map, which you can use to highlight regions of interest.

## Topics

### Accessing the Results

var results: [VNSaliencyImageObservation]?

The results of the image saliency request.

### Identifying Request Revisions

let VNGenerateObjectnessBasedSaliencyImageRequestRevision1: Int

A constant for specifying revision 1 of the image saliency request.

## Relationships

### Inherits From

- VNImageBasedRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Saliency analysis

Cropping Images Using Saliency

Isolate regions in an image that are most likely to draw people’s attention.

Highlighting Areas of Interest in an Image Using Saliency

Quantify and visualize where people are likely to look in an image.

class VNGenerateAttentionBasedSaliencyImageRequest

An object that produces a heat map that identifies the parts of an image most likely to draw attention.

class VNSaliencyImageObservation

An observation that contains a grayscale heat map of important areas across an image.

