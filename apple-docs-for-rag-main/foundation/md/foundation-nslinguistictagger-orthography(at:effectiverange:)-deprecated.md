

- Foundation
- NSLinguisticTagger
-  orthography(at:effectiveRange:) Deprecated

Instance Method

# orthography(at:effectiveRange:)

Returns the orthography at the index and also returns the effective range.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func orthography(
    at charIndex: Int,
    effectiveRange: NSRangePointer?
) -> NSOrthography?
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`charIndex`  

The character index to begin examination.

`effectiveRange`  

An NSRangePointer that, upon completion, contains the range of the orthography containing `charIndex`.

## Return Value

The orthography for the location.

## See Also

### Determining the Dominant Language and Orthography

class func dominantLanguage(for: String) -> String?

Returns the dominant language for the specified string.

Deprecated

var dominantLanguage: String?

Returns the dominant language of the string set for the linguistic tagger.

Deprecated

func setOrthography(NSOrthography?, range: NSRange)

Sets the orthography for the specified range.

Deprecated

