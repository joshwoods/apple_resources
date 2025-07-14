

- Foundation
- NSLinguisticTagger
-  tokenRange(at:unit:) Deprecated

Instance Method

# tokenRange(at:unit:)

Returns the range of the linguistic unit containing the specified character index.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.13–15.4DeprecatedtvOS 11.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 4.0–9.0Deprecated

``` source
func tokenRange(
    at charIndex: Int,
    unit: NSLinguisticTaggerUnit
) -> NSRange
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`charIndex`  

The character index to begin examination.

`unit`  

The linguistic unit. For possible values, see NSLinguisticTaggerUnit.

## Return Value

The range of the substring for the linguistic unit.

## See Also

### Determining the Range of a Unit Token

func sentenceRange(for: NSRange) -> NSRange

Returns the range of a sentence containing the specified range.

Deprecated

