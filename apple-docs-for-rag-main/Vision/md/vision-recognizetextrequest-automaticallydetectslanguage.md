

- Vision
- RecognizeTextRequest
-  automaticallyDetectsLanguage 

Instance Property

# automaticallyDetectsLanguage

A Boolean value that indicates whether to attempt detecting the language to use the appropriate model for recognition and language correction.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var automaticallyDetectsLanguage: Bool
```

## See Also

### Inspecting a request

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

enum RecognitionLevel

Constants that identify the performance and accuracy of the text recognition.

