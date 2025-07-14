

- Vision
- VNRecognizeTextRequest
-  usesLanguageCorrection 

Instance Property

# usesLanguageCorrection

A Boolean value that indicates whether the request applies language correction during the recognition process.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var usesLanguageCorrection: Bool { get set }
```

## Discussion

When this value is true, Vision applies language correction during the recognition process. Disabling this property returns the raw recognition results, which provides performance benefits but less accurate results.

## See Also

### Specifying the Language

var automaticallyDetectsLanguage: Bool

A Boolean value that indicates whether to attempt detecting the language to use the appropriate model for recognition and language correction.

var recognitionLanguages: [String]

An array of languages to detect, in priority order.

var customWords: [String]

An array of strings to supplement the recognized languages at the word-recognition stage.

func supportedRecognitionLanguages() throws -> [String]

Returns the identifiers of the languages that the request supports.

class func supportedRecognitionLanguages(for: VNRequestTextRecognitionLevel, revision: Int) throws -> [String]

Requests a list of languages that the specified revision recognizes.

Deprecated

