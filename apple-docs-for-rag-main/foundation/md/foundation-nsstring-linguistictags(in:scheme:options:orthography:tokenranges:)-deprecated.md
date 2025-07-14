

- Foundation
- NSString
-  linguisticTags(in:scheme:options:orthography:tokenRanges:) Deprecated

Instance Method

# linguisticTags(in:scheme:options:orthography:tokenRanges:)

Returns an array of linguistic tags for the specified range and requested tags within the receiving string.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func linguisticTags(
    in range: NSRange,
    scheme: NSLinguisticTagScheme,
    options: NSLinguisticTagger.Options = [],
    orthography: NSOrthography?,
    tokenRanges: AutoreleasingUnsafeMutablePointer?
) -> [NSLinguisticTag]
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`range`  

The range of the string to analyze.

`scheme`  

The tag scheme to use. See Linguistic Tag Schemes for supported values.

`options`  

The linguistic tagger options to use. See NSLinguisticTagger.Options for the constants. These constants can be combined using the C-Bitwise OR operator.

`orthography`  

The orthography of the string. If `nil`, the linguistic tagger will attempt to determine the orthography from the string content.

`tokenRanges`  

An array returned by-reference containing the token ranges of the linguistic tags wrapped in `NSValue` objects.

## Return Value

Returns an array containing the linguistic tags for the `tokenRanges` within the receiving string.

## Discussion

This is a convenience method. It is the equivalent of creating an instance of NSLinguisticTagger, specifying the receiver as the string to be analyzed, and the orthography (or `nil`) and then invoking the NSLinguisticTagger method or linguisticTags(in:scheme:options:orthography:tokenRanges:).

## See Also

### Performing Linguistic Analysis

func enumerateLinguisticTags(in: NSRange, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, using: (NSLinguisticTag?, NSRange, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Performs linguistic analysis on the specified string by enumerating the specific range of the string, providing the Block with the located tags.

Deprecated

struct EnumerationOptions

Constants to specify kinds of substrings and styles of enumeration.

