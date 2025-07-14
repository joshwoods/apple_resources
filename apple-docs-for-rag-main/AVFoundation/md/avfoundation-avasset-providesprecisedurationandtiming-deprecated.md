

- AVFoundation
- AVAsset
-  providesPreciseDurationAndTiming Deprecated

Instance Property

# providesPreciseDurationAndTiming

A Boolean value that indicates whether the asset provides precise duration and timing.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var providesPreciseDurationAndTiming: Bool { get }
```

Deprecated

Load the value of providesPreciseDurationAndTiming asynchronously instead.

## Discussion

This property value is true if you initialized the asset with the AVURLAssetPreferPreciseDurationAndTimingKey initialization option, otherwise it’s false.

