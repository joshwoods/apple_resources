

- Vision
-  VNDetectRectanglesRequest 

Class

# VNDetectRectanglesRequest

An image-analysis request that finds projected rectangular regions in an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNDetectRectanglesRequest
```

## Overview

A rectangle detection request locates regions of an image with rectangular shape, like credit cards, business cards, documents, and signs. The request returns its observations in the form of VNRectangleObservation objects, which contain normalized coordinates of bounding boxes containing the rectangle.

Use this type of request to find the bounding boxes of rectangles in an image. Vision returns observations for rectangles found in all orientations and sizes, along with a confidence level to indicate how likely it’s that the observation contains an actual rectangle.

To further configure or restrict the types of rectangles found, set properties on the request specifying a range of aspect ratios, sizes, and quadrature tolerance.

## Topics

### Configuring Detection

var minimumAspectRatio: VNAspectRatio

A `float` specifying the minimum aspect ratio of the rectangle to detect, defined as the shorter dimension over the longer dimension.

var maximumAspectRatio: VNAspectRatio

A `float` specifying the maximum aspect ratio of the rectangle to detect, defined as the shorter dimension over the longer dimension.

typealias VNAspectRatio

A type alias for expressing rectangle aspect ratios in Vision.

var quadratureTolerance: VNDegrees

A float specifying the number of degrees a rectangle corner angle can deviate from 90°.

typealias VNDegrees

A typealias for expressing tolerance angles in Vision.

var minimumSize: Float

The minimum size of a rectangle to detect, as a proportion of the smallest dimension.

var minimumConfidence: VNConfidence

A value specifying the minimum acceptable confidence level.

typealias VNConfidence

A type alias for the confidence value of an observation.

var maximumObservations: Int

An integer specifying the maximum number of rectangles Vision returns.

### Accessing the Results

var results: [VNRectangleObservation]?

The results of the request to detect rectangles.

class VNRectangleObservation

An object that represents the four vertices of a detected rectangle.

### Identifying Request Revisions

let VNDetectRectanglesRequestRevision1: Int

A constant for specifying revision 1 of the rectangle detection request.

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

