

- Vision
- VNRecognizeTextRequest
-  supportedRecognitionLanguages(for:revision:) Deprecated

Type Method

# supportedRecognitionLanguages(for:revision:)

Requests a list of languages that the specified revision recognizes.

iOS 13.0–15.0DeprecatediPadOS 13.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.15–12.0DeprecatedtvOS 13.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func supportedRecognitionLanguages(
    for recognitionLevel: VNRequestTextRecognitionLevel,
    revision requestRevision: Int
) throws -> [String]
```

Deprecated

Use supportedRecognitionLanguages() instead.

## Parameters 

`recognitionLevel`  

The level of recognition to prioritize. Set this level to VNRequestTextRecognitionLevel.fastto prioritize speed over accuracy, and to VNRequestTextRecognitionLevel.accurate to prioritize accuracy at the expense of speed.

`requestRevision`  

The revision of the text recognition algorithm for the Vision framework to use.

## Return Value

An array of supported languages, listed as ISO language codes.

## Mentioned in 

Recognizing Text in Images

## Discussion

A language supported in one recognition level may not be available in another recognition level.

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

func supportedRecognitionLanguages() throws -> [String]

Returns the identifiers of the languages that the request supports.

