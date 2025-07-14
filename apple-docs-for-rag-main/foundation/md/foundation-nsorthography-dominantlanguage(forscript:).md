

- Foundation
- NSOrthography
-  dominantLanguage(forScript:) 

Instance Method

# dominantLanguage(forScript:)

Returns the dominant language for the specified script.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dominantLanguage(forScript script: String) -> String?
```

## Parameters 

`script`  

The specified script.

## Discussion

The value of this property is a BCP-47 language tag, such as `"en"` or `"fr"`, that identifies the dominant language.

## See Also

### Determining Correspondences Between Languages and Scripts

var languageMap: [String : [String]]

A dictionary that maps script tags to arrays of language tags.

var dominantLanguage: String

The first language in the list of languages for the dominant script.

var dominantScript: String

The dominant script for the text.

func languages(forScript: String) -> [String]?

Returns the list of languages for the specified script.

var allScripts: [String]

The scripts appearing as keys in the language map.

var allLanguages: [String]

The languages appearing in values of the language map.

