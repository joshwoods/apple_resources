

- Foundation
- NSLinguisticTagger
-  tags(in:scheme:options:tokenRanges:) Deprecated

Instance Method

# tags(in:scheme:options:tokenRanges:)

Returns an array of linguistic tags and token ranges for a given string range.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func tags(
    in range: NSRange,
    scheme tagScheme: String,
    options opts: NSLinguisticTagger.Options = [],
    tokenRanges: AutoreleasingUnsafeMutablePointer?
) -> [String]
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`range`  

The range from which to return tags.

`tagScheme`  

The tag scheme. See NSLinguisticTagScheme for possible values.

`opts`  

The linguistic tagger options to use. See NSLinguisticTagger.Options for possible values.

`tokenRanges`  

Returns by reference an array of token ranges.

## Return Value

An array of the tags in the requested range.

## Discussion

When the returned array contains an entry that doesn’t have a corresponding tag scheme, that entry is an empty string (`""`).

This is a convenience method for calling tags(in:unit:scheme:options:tokenRanges:) and passing NSLinguisticTaggerUnit.word as the linguistic unit.

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

class func tags(for: String, range: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [NSLinguisticTag]

Returns an array of linguistic tags and token ranges for a given string and linguistic unit.

Deprecated

