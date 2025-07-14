

- Vision
- VNRecognizeTextRequest
-  automaticallyDetectsLanguage 

Instance Property

# automaticallyDetectsLanguage

A Boolean value that indicates whether to attempt detecting the language to use the appropriate model for recognition and language correction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var automaticallyDetectsLanguage: Bool { get set }
```

## See Also

### Specifying the Language

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

