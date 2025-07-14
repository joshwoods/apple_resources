

- AVFoundation
- AVMutableComposition
-  insertTimeRange(\_:of:at:) Deprecated

Instance Method

# insertTimeRange(\_:of:at:)

Inserts all the tracks within a given time range of a specified asset into the composition.

iOS 4.0–18.0DeprecatediPadOS 4.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 1.0–11.0Deprecated

``` source
func insertTimeRange(
    _ timeRange: CMTimeRange,
    of asset: AVAsset,
    at startTime: CMTime
) throws
```

Deprecated

Use insertTimeRange(_:of:at:isolation:) instead.

## Parameters 

`timeRange`  

The time range of the asset to be inserted.

`asset`  

An asset that contains the tracks to be inserted.

`startTime`  

The time at which the inserted tracks should be presented by the receiver.

## Discussion

This method may add new tracks to ensure that all tracks of the asset are represented in the inserted time range.

Existing content at the specified start time is pushed out by the duration of the time range.

Media data for the inserted time range is presented at its natural duration; you can scale it to a different duration using scaleTimeRange(_:toDuration:).

## See Also

### Managing Time Ranges

func removeTimeRange(CMTimeRange)

Removes a specified time range from all tracks of the composition.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of all tracks in a given time range.

func insertEmptyTimeRange(CMTimeRange)

Adds or extends an empty time range within all tracks of the composition.

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime, completionHandler: ((any Error)?) -> Void)

Inserts all tracks of an asset for a time range into a composition.

Deprecated

