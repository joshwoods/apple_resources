

- AVFoundation
- AVAssetTrack
-  segment(forTrackTime:) Deprecated

Instance Method

# segment(forTrackTime:)

Retrieves a segment with a target time range that contains, or is closest to, the specified track time.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func segment(forTrackTime trackTime: CMTime) -> AVAssetTrackSegment?
```

Deprecated

Use loadSegment(forTrackTime:completionHandler:) instead.

## Parameters 

`trackTime`  

The track time for which you want the segment.

## Return Value

The track segment matching, or closest to, the specied time.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load a segment asynchronously using loadSegment(forTrackTime:completionHandler:) instead.

