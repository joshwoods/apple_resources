

- AVFoundation
- AVAssetTrack
-  totalSampleDataLength Deprecated

Instance Property

# totalSampleDataLength

The total number of bytes of sample data the track requires.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var totalSampleDataLength: Int64 { get }
```

Deprecated

Load the value of totalSampleDataLength asynchronously instead.

## Discussion

The value may be `0` if the framework can’t determine the total sample data length.

