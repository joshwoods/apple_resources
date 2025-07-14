

- Foundation
- NSLinguisticTagger
-  init(tagSchemes:options:) Deprecated

Initializer

# init(tagSchemes:options:)

Creates a linguistic tagger instance using the specified tag schemes and options.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
init(
    tagSchemes: [NSLinguisticTagScheme],
    options opts: Int
)
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`tagSchemes`  

An array of tag schemes to be used. See NSLinguisticTagScheme for the possible values.

`opts`  

Reserved for future use. Specify `0` for this parameter.

## Return Value

An initialized linguistic tagger.

## Discussion

Pass any tag schemes to `tagSchemes` that you intend to use with the methods described in Enumerating Linguistic Tags and Getting Linguistic Tags.

Tip

Avoid specifying tag schemes that you won’t use to ensure optimal performance.

## See Also

### Related Documentation

struct NSLinguisticTagScheme

Constants for the tag schemes specified when initializing a linguistic tagger.

### First Steps

Tokenizing Natural Language Text

Enumerate the words in a string.

var string: String?

The string being analyzed by the linguistic tagger.

Deprecated

