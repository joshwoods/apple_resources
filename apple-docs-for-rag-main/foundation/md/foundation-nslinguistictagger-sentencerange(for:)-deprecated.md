

- Foundation
- NSLinguisticTagger
-  sentenceRange(for:) Deprecated

Instance Method

# sentenceRange(for:)

Returns the range of a sentence containing the specified range.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func sentenceRange(for range: NSRange) -> NSRange
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`range`  

The character range.

## Return Value

Returns the range of the sentence.

## Discussion

This is a convenience method for calling tokenRange(at:unit:), passing the NSLinguisticTaggerUnit.sentence unit and the first position of the provided range.

## See Also

### Determining the Range of a Unit Token

func tokenRange(at: Int, unit: NSLinguisticTaggerUnit) -> NSRange

Returns the range of the linguistic unit containing the specified character index.

Deprecated

