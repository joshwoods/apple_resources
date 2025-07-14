

- Foundation
- NSLinguisticTagger
-  availableTagSchemes(forLanguage:) Deprecated

Type Method

# availableTagSchemes(forLanguage:)

Returns the tag schemes available for a particular language on the current device.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
class func availableTagSchemes(forLanguage language: String) -> [NSLinguisticTagScheme]
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`language`  

A BCP-47 tag identifying the language. For example, “en” for English or “zh-Hans” for Chinese written using the Simplified Chinese script.

## Return Value

The available tag schemes. For possible values, see NSLinguisticTagScheme.

## Discussion

This is a convenience method for calling the availableTagSchemes(for:language:), passing NSLinguisticTaggerUnit.word as the linguistic unit.

## See Also

### Getting the Tag Schemes

class func availableTagSchemes(for: NSLinguisticTaggerUnit, language: String) -> [NSLinguisticTagScheme]

Returns the tag schemes available for a particular unit and language on the current device.

Deprecated

var tagSchemes: [NSLinguisticTagScheme]

Returns the tag schemes configured for this linguistic tagger. For possible values, see NSLinguisticTagScheme.

Deprecated

