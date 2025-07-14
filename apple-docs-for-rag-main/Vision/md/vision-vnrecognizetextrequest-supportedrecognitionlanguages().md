

- Vision
- VNRecognizeTextRequest
-  supportedRecognitionLanguages() 

Instance Method

# supportedRecognitionLanguages()

Returns the identifiers of the languages that the request supports.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func supportedRecognitionLanguages() throws -> [String]
```

## Return Value

The language identifiers.

## See Also

### Specifying the Language

var automaticallyDetectsLanguage: Bool

A Boolean value that indicates whether to attempt detecting the language to use the appropriate model for recognition and language correction.

var recognitionLanguages: [String]

An array of languages to detect, in priority order.

var usesLanguageCorrection: Bool

A Boolean value that indicates whether the request applies language correction during the recognition process.

var customWords: [String]

An array of strings to supplement the recognized languages at the word-recognition stage.

class func supportedRecognitionLanguages(for: VNRequestTextRecognitionLevel, revision: Int) throws -> [String]

Requests a list of languages that the specified revision recognizes.

Deprecated

