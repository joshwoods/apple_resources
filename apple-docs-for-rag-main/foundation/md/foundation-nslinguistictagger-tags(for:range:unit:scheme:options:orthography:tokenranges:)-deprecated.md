

- Foundation
- NSLinguisticTagger
-  tags(for:range:unit:scheme:options:orthography:tokenRanges:) Deprecated

Type Method

# tags(for:range:unit:scheme:options:orthography:tokenRanges:)

Returns an array of linguistic tags and token ranges for a given string and linguistic unit.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.13–15.4DeprecatedtvOS 11.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 4.0–9.0Deprecated

``` source
class func tags(
    for string: String,
    range: NSRange,
    unit: NSLinguisticTaggerUnit,
    scheme: NSLinguisticTagScheme,
    options: NSLinguisticTagger.Options = [],
    orthography: NSOrthography?,
    tokenRanges: AutoreleasingUnsafeMutablePointer?
) -> [NSLinguisticTag]
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`string`  

The range from which to return tags.

`range`  

The linguistic unit. See NSLinguisticTaggerUnit for possible values.

`unit`  

The tag scheme. See NSLinguisticTagScheme for possible values.

`scheme`  

The linguistic tagger options to use. See NSLinguisticTagger.Options for possible values.

`options`  

Returns by reference an array of token ranges.

## Return Value

An array of the tags in the requested range.

## Discussion

When the returned array contains an entry that doesn’t have a corresponding tag scheme, that entry is an empty string (`""`).

This is a convenience method for initializing a linguistic tagger, setting the string property, and calling the tags(in:unit:scheme:options:tokenRanges:) method. If you analyze the same string more than once, you should create a linguistic tagger object instead of calling this method.

## See Also

### Getting Linguistic Tags

func tag(at: Int, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, tokenRange: NSRangePointer?) -> NSLinguisticTag?

Returns a tag for a single scheme, for a given linguistic unit, at the specified character position.

Deprecated

func tag(at: Int, scheme: NSLinguisticTagScheme, tokenRange: NSRangePointer?, sentenceRange: NSRangePointer?) -> NSLinguisticTag?

Returns a tag for a single scheme at the specified character position.

Deprecated

class func tag(for: String, at: Int, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, orthography: NSOrthography?, tokenRange: NSRangePointer?) -> NSLinguisticTag?

Returns a tag for a single scheme, for a given linguistic unit, at the specified character position in a string.

Deprecated

func tags(in: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [NSLinguisticTag]

Returns an array of linguistic tags and token ranges for a given string range and linguistic unit.

Deprecated

func tags(in: NSRange, scheme: String, options: NSLinguisticTagger.Options, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [String]

Returns an array of linguistic tags and token ranges for a given string range.

Deprecated

