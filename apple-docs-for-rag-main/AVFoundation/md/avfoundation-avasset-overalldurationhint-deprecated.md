

- AVFoundation
- AVAsset
-  overallDurationHint Deprecated

Instance Property

# overallDurationHint

The total duration of fragments that currently exist, or may exist in the future.

iOS 10.2–16.0DeprecatediPadOS 10.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.12.2–13.0DeprecatedtvOS 10.2–16.0DeprecatedwatchOS 3.2–9.0Deprecated

``` source
var overallDurationHint: CMTime { get }
```

Deprecated

Load the value of overallDurationHint asynchronously instead.

## Discussion

For QuickTime movie files and MPEG-4 files, the asset retrieves this value from the `mehd` box of the `mvex` box, if present. If no total fragment duration hint is available, the value of this property is invalid.

