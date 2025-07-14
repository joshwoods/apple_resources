

- Vision
-  VNRecognizedTextObservation 

Class

# VNRecognizedTextObservation

A request that detects and recognizes regions of text in an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNRecognizedTextObservation
```

## Mentioned in 

Recognizing Text in Images

## Overview

This type of observation results from a VNRecognizeTextRequest. It contains information about both the location and content of text and glyphs that Vision recognized in the input image.

## Topics

### Obtaining Recognized Text

func topCandidates(Int) -> [VNRecognizedText]

Requests the *n* top candidates for a recognized text string.

class VNRecognizedText

Text recognized in an image through a text recognition request.

## Relationships

### Inherits From

- VNRectangleObservation

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

### Text recognition

Recognizing Text in Images

Add text-recognition features to your app using the Vision framework.

Structuring Recognized Text on a Document

Detect, recognize, and structure text on a business card or receipt using Vision and VisionKit.

Extracting phone numbers from text in images

Analyze and filter phone numbers from text in live capture by using Vision.

Locating and displaying recognized text

Perform text recognition on a photo using the Vision framework’s text-recognition request.

class VNRecognizeTextRequest

An image-analysis request that finds and recognizes text in an image.

