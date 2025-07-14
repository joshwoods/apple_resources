

- Vision
- VNRecognizeTextRequest
-  recognitionLanguages 

Instance Property

# recognitionLanguages

An array of languages to detect, in priority order.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var recognitionLanguages: [String] { get set }
```

## Mentioned in 

Recognizing Text in Images

## Discussion

The order of the languages in the array defines the order in which languages are used during language processing and text recognition.

Specify the languages as ISO language codes.

## See Also

### Specifying the Language

var automaticallyDetectsLanguage: Bool

A Boolean value that indicates whether to attempt detecting the language to use the appropriate model for recognition and language correction.

var usesLanguageCorrection: Bool

A Boolean value that indicates whether the request applies language correction during the recognition process.

var customWords: [String]

An array of strings to supplement the recognized languages at the word-recognition stage.

func supportedRecognitionLanguages() throws -> [String]

Returns the identifiers of the languages that the request supports.

class func supportedRecognitionLanguages(for: VNRequestTextRecognitionLevel, revision: Int) throws -> [String]

Requests a list of languages that the specified revision recognizes.

Deprecated

