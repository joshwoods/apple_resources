

- Foundation
- NSLinguisticTagger
-  availableTagSchemes(for:language:) Deprecated

Type Method

# availableTagSchemes(for:language:)

Returns the tag schemes available for a particular unit and language on the current device.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.13–15.4DeprecatedtvOS 11.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 4.0–9.0Deprecated

``` source
class func availableTagSchemes(
    for unit: NSLinguisticTaggerUnit,
    language: String
) -> [NSLinguisticTagScheme]
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`unit`  

The linguistic unit. For possible values, see NSLinguisticTaggerUnit.

`language`  

A BCP-47 tag identifying the language. For example, “en” for English or “zh-Hans” for Chinese written using the Simplified Chinese script.

## Return Value

The supported tag schemes. For possible values, see NSLinguisticTagScheme.

## See Also

### Getting the Tag Schemes

class func availableTagSchemes(forLanguage: String) -> [NSLinguisticTagScheme]

Returns the tag schemes available for a particular language on the current device.

Deprecated

var tagSchemes: [NSLinguisticTagScheme]

Returns the tag schemes configured for this linguistic tagger. For possible values, see NSLinguisticTagScheme.

Deprecated

