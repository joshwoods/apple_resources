

- AVFoundation
- AVMutableComposition
-  insertTimeRange(\_:of:at:completionHandler:) Deprecated

Instance Method

# insertTimeRange(\_:of:at:completionHandler:)

Inserts all tracks of an asset for a time range into a composition.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func insertTimeRange(
    _ timeRange: CMTimeRange,
    of asset: AVAsset,
    at startTime: CMTime,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

Deprecated

Use insertTimeRange(_:of:at:isolation:) instead.

## Parameters 

`timeRange`  

The time range of the asset’s tracks to insert into the composition.

`asset`  

The source asset that contains the tracks to insert.

`startTime`  

A time in the composition to present the inserted tracks.

`completionHandler`  

A callback the system invokes when the insertion is complete. If an error occurs, the system passes the callback an error object that describes the failure.

## Discussion

If necessary, a composition adds new tracks to ensure that it inserts all tracks in the source asset for the time range. Inserting a time range pushes out existing content at the specified start time by the time range’s duration.

The composition presents the media data for the inserted time range at its natural duration and rate. You can scale it to a different duration, which changes the presentation rate, by calling scaleTimeRange(_:toDuration:).

## See Also

### Managing Time Ranges

func removeTimeRange(CMTimeRange)

Removes a specified time range from all tracks of the composition.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of all tracks in a given time range.

func insertEmptyTimeRange(CMTimeRange)

Adds or extends an empty time range within all tracks of the composition.

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime) throws

Inserts all the tracks within a given time range of a specified asset into the composition.

Deprecated

