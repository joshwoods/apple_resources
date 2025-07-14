

- Vision
-  VNRecognizeTextRequest 

Class

# VNRecognizeTextRequest

An image-analysis request that finds and recognizes text in an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNRecognizeTextRequest
```

## Mentioned in 

Recognizing Text in Images

## Overview

By default, a text recognition request first locates all possible glyphs or characters in the input image, and then analyzes each string. To specify or limit the languages to find in the request, set the recognitionLanguages property to an array that contains the names of the languages of text you want to recognize. Vision returns the result of this request in a VNRecognizedTextObservation object.

## Topics

### Customizing Recognition Constraints

var minimumTextHeight: Float

The minimum height, relative to the image height, of the text to recognize.

var recognitionLevel: VNRequestTextRecognitionLevel

A value that determines whether the request prioritizes accuracy or speed in text recognition.

enum VNRequestTextRecognitionLevel

Constants that identify the performance and accuracy of the text recognition.

### Accessing the Results

var results: [VNRecognizedTextObservation]?

The results of the text recognition request.

### Specifying the Language

var automaticallyDetectsLanguage: Bool

A Boolean value that indicates whether to attempt detecting the language to use the appropriate model for recognition and language correction.

var recognitionLanguages: [String]

An array of languages to detect, in priority order.

var usesLanguageCorrection: Bool

A Boolean value that indicates whether the request applies language correction during the recognition process.

var customWords: [String]

An array of strings to supplement the recognized languages at the word-recognition stage.

func supportedRecognitionLanguages() throws -> [String]

Returns the identifiers of the languages that the request supports.

class func supportedRecognitionLanguages(for: VNRequestTextRecognitionLevel, revision: Int) throws -> [String]

Requests a list of languages that the specified revision recognizes.

Deprecated

### Identifying Request Revisions

let VNRecognizeTextRequestRevision3: Int

A constant for specifying revision 3 of the text recognition request.

let VNRecognizeTextRequestRevision2: Int

A constant for specifying revision 2 of the text recognition request.

Deprecated

let VNRecognizeTextRequestRevision1: Int

A constant for specifying revision 1 of the text recognition request.

Deprecated

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
- VNRequestProgressProviding

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

class VNRecognizedTextObservation

A request that detects and recognizes regions of text in an image.

