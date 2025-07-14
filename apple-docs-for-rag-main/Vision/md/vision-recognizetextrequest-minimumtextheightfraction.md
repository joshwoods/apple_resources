

- Vision
- RecognizeTextRequest
-  minimumTextHeightFraction 

Instance Property

# minimumTextHeightFraction

The minimum height, relative to the image height, of the text to recognize.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var minimumTextHeightFraction: Float
```

## Discussion

Specify a floating-point number relative to the image height. For example, to limit recognition to text that’s half of the image height, use `0.5`. Increasing the size reduces memory consumption and expedites recognition with the tradeoff of ignoring text smaller than the minimum height. The default value is `1/32`, or `0.03125`.

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

var recognitionLanguages: [Locale.Language]

An array of languages to detect, in priority order.

var recognitionLevel: RecognizeTextRequest.RecognitionLevel

A value that determines whether the request prioritizes accuracy or speed in text recognition.

enum RecognitionLevel

Constants that identify the performance and accuracy of the text recognition.

