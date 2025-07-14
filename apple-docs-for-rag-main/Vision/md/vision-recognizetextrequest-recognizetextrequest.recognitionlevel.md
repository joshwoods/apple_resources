

- Vision
- RecognizeTextRequest
-  RecognizeTextRequest.RecognitionLevel 

Enumeration

# RecognizeTextRequest.RecognitionLevel

Constants that identify the performance and accuracy of the text recognition.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum RecognitionLevel
```

## Topics

### Getting the recognition levels

case accurate

Accurate text recognition takes more time to produce a more comprehensive result.

case fast

Fast text recognition returns results more quickly at the expense of accuracy.

## Relationships

### Conforms To

- CaseIterable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting a request

var automaticallyDetectsLanguage: Bool

A Boolean value that indicates whether to attempt detecting the language to use the appropriate model for recognition and language correction.

var usesLanguageCorrection: Bool

A Boolean value that indicates whether the request applies language correction during the recognition process.

var supportedRecognitionLanguages: [Locale.Language]

The identifiers of the languages that the request supports.

var customWords: [String]

An array of strings to supplement the recognized languages at the word-recognition stage.

var minimumTextHeightFraction: Float

The minimum height, relative to the image height, of the text to recognize.

var recognitionLanguages: [Locale.Language]

An array of languages to detect, in priority order.

var recognitionLevel: RecognizeTextRequest.RecognitionLevel

A value that determines whether the request prioritizes accuracy or speed in text recognition.

