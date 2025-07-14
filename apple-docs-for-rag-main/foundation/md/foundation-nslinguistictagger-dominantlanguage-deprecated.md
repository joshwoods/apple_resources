

- Foundation
- NSLinguisticTagger
-  dominantLanguage Deprecated

Instance Property

# dominantLanguage

Returns the dominant language of the string set for the linguistic tagger.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.13–15.4DeprecatedtvOS 11.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 4.0–9.0Deprecated

``` source
var dominantLanguage: String? { get }
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Return Value

The BCP-47 tag identifying the dominant language of the string, or the tag “und” if a specific language cannot be determined.

## Discussion

If you want to know the dominant language of a string that you’re analyzing with a linguistic tagger (for example, identifying part of speech for each word), specify the language tag scheme in the initializer. After you set the string property of the linguistic tagger, the dominant language can be determined with the dominantLanguage property, as shown in this example:

```
let text = "Die Kleinen haben friedlich zusammen gespielt."
let tagger = NSLinguisticTagger(tagSchemes: [.language], options: 0)
tagger.string = text
tagger.dominantLanguage // "de"
```

In the example, the BCP-47 language tag “de” is returned as the dominant language, indicating that the text is in German.

## See Also

### Determining the Dominant Language and Orthography

class func dominantLanguage(for: String) -> String?

Returns the dominant language for the specified string.

Deprecated

func orthography(at: Int, effectiveRange: NSRangePointer?) -> NSOrthography?

Returns the orthography at the index and also returns the effective range.

Deprecated

func setOrthography(NSOrthography?, range: NSRange)

Sets the orthography for the specified range.

Deprecated

