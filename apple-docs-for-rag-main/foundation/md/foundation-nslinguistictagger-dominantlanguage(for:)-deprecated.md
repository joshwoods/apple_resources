

- Foundation
- NSLinguisticTagger
-  dominantLanguage(for:) Deprecated

Type Method

# dominantLanguage(for:)

Returns the dominant language for the specified string.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.13–15.4DeprecatedtvOS 11.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 4.0–9.0Deprecated

``` source
class func dominantLanguage(for string: String) -> String?
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`string`  

The string for which the dominant language is determined.

## Return Value

The BCP-47 tag identifying the dominant language of the string, or the tag “und” if a specific language cannot be determined.

## Discussion

The dominantLanguage(for:) method is a convenience method for creating a new linguistic tagger, setting the string property, and getting the dominantLanguage property. If you analyze the same string more than once, create a linguistic tagger object instead of calling the method, as shown in this example:

```
let text = "Die Kleinen haben friedlich zusammen gespielt."
NSLinguisticTagger.dominantLanguage(for: text) // "de"
```

In the example, the BCP-47 language tag “de” is returned as the dominant language, indicating that the text is in German.

## See Also

### Determining the Dominant Language and Orthography

var dominantLanguage: String?

Returns the dominant language of the string set for the linguistic tagger.

Deprecated

func orthography(at: Int, effectiveRange: NSRangePointer?) -> NSOrthography?

Returns the orthography at the index and also returns the effective range.

Deprecated

func setOrthography(NSOrthography?, range: NSRange)

Sets the orthography for the specified range.

Deprecated

