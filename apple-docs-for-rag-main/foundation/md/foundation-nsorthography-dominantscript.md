

- Foundation
- NSOrthography
-  dominantScript 

Instance Property

# dominantScript

The dominant script for the text.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var dominantScript: String { get }
```

## Discussion

The value of this property is an ISO 15924 script code, such as `"Latn"` or `"Cyrl"`, that identifies the dominant script.

## See Also

### Determining Correspondences Between Languages and Scripts

var languageMap: [String : [String]]

A dictionary that maps script tags to arrays of language tags.

var dominantLanguage: String

The first language in the list of languages for the dominant script.

func dominantLanguage(forScript: String) -> String?

Returns the dominant language for the specified script.

func languages(forScript: String) -> [String]?

Returns the list of languages for the specified script.

var allScripts: [String]

The scripts appearing as keys in the language map.

var allLanguages: [String]

The languages appearing in values of the language map.

