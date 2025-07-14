

- Foundation
- NSLinguisticTagger
-  setOrthography(\_:range:) Deprecated

Instance Method

# setOrthography(\_:range:)

Sets the orthography for the specified range.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func setOrthography(
    _ orthography: NSOrthography?,
    range: NSRange
)
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`orthography`  

The orthography.

`range`  

The range.

## Discussion

If the orthography of the linguistic tagger is not set, it will determine it automatically from the contents of the text. You should call this method only if you know the orthography of the text by some other means.

## See Also

### Determining the Dominant Language and Orthography

class func dominantLanguage(for: String) -> String?

Returns the dominant language for the specified string.

Deprecated

var dominantLanguage: String?

Returns the dominant language of the string set for the linguistic tagger.

Deprecated

func orthography(at: Int, effectiveRange: NSRangePointer?) -> NSOrthography?

Returns the orthography at the index and also returns the effective range.

Deprecated

