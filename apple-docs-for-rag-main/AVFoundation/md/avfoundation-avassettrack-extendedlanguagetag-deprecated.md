

- AVFoundation
- AVAssetTrack
-  extendedLanguageTag Deprecated

Instance Property

# extendedLanguageTag

The language tag of the track.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var extendedLanguageTag: String? { get }
```

Deprecated

Load the value of extendedLanguageTag asynchronously instead.

## Discussion

The value is a BCP-47 language tag, or `nil` if the track doesn’t specify a language tag.

