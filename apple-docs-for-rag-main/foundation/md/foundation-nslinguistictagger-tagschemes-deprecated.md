

- Foundation
- NSLinguisticTagger
-  tagSchemes Deprecated

Instance Property

# tagSchemes

Returns the tag schemes configured for this linguistic tagger. For possible values, see NSLinguisticTagScheme.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
var tagSchemes: [NSLinguisticTagScheme] { get }
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## See Also

### Getting the Tag Schemes

class func availableTagSchemes(for: NSLinguisticTaggerUnit, language: String) -> [NSLinguisticTagScheme]

Returns the tag schemes available for a particular unit and language on the current device.

Deprecated

class func availableTagSchemes(forLanguage: String) -> [NSLinguisticTagScheme]

Returns the tag schemes available for a particular language on the current device.

Deprecated

