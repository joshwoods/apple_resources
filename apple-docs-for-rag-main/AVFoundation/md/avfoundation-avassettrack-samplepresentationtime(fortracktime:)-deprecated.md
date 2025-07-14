

- AVFoundation
- AVAssetTrack
-  samplePresentationTime(forTrackTime:) Deprecated

Instance Method

# samplePresentationTime(forTrackTime:)

Maps the specified track time through the appropriate time mapping and returns the resulting sample presentation time.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func samplePresentationTime(forTrackTime trackTime: CMTime) -> CMTime
```

Deprecated

Use loadSamplePresentationTime(forTrackTime:completionHandler:) instead.

## Parameters 

`trackTime`  

The track time for which to request the sample presentation time.

## Return Value

The sample presentation time corresponding to the specified time; otherwise invalid if the time is out of range.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load a sample presentation time asynchronously using loadSamplePresentationTime(forTrackTime:completionHandler:) instead.

