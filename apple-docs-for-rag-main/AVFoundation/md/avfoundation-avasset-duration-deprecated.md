

- AVFoundation
- AVAsset
-  duration Deprecated

Instance Property

# duration

A time value that indicates the asset’s duration.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var duration: CMTime { get }
```

Deprecated

Load the value of duration asynchronously instead.

## Discussion

If you initialized the asset by passing the AVURLAssetPreferPreciseDurationAndTimingKey initialization option, this property value provides the asset’s precise duration; otherwise, it provides a best-available estimate. You can determine the value’s accuracy by querying the asset’s providesPreciseDurationAndTiming property.

