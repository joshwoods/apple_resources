

- Vision
- VNRecognizeTextRequest
-  customWords 

Instance Property

# customWords

An array of strings to supplement the recognized languages at the word-recognition stage.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var customWords: [String] { get set }
```

## Mentioned in 

Recognizing Text in Images

## Discussion

Custom words take precedence over the standard lexicon. The request ignores this value if usesLanguageCorrection is false.

## See Also

### Specifying the Language

var automaticallyDetectsLanguage: Bool

A Boolean value that indicates whether to attempt detecting the language to use the appropriate model for recognition and language correction.

var recognitionLanguages: [String]

An array of languages to detect, in priority order.

var usesLanguageCorrection: Bool

A Boolean value that indicates whether the request applies language correction during the recognition process.

func supportedRecognitionLanguages() throws -> [String]

Returns the identifiers of the languages that the request supports.

class func supportedRecognitionLanguages(for: VNRequestTextRecognitionLevel, revision: Int) throws -> [String]

Requests a list of languages that the specified revision recognizes.

Deprecated

