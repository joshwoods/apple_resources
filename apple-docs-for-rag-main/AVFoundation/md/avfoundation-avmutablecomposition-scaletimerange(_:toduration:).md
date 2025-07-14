

- AVFoundation
- AVMutableComposition
-  scaleTimeRange(\_:toDuration:) 

Instance Method

# scaleTimeRange(\_:toDuration:)

Changes the duration of all tracks in a given time range.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func scaleTimeRange(
    _ timeRange: CMTimeRange,
    toDuration duration: CMTime
)
```

## Parameters 

`timeRange`  

The time range of the composition to scale.

`duration`  

The new time range duration.

## Discussion

A composition presents each track segment affected by the scaling operation at a rate equal to `source.duration / target.duration` of its resulting time mapping.

## See Also

### Managing Time Ranges

func removeTimeRange(CMTimeRange)

Removes a specified time range from all tracks of the composition.

func insertEmptyTimeRange(CMTimeRange)

Adds or extends an empty time range within all tracks of the composition.

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime, completionHandler: ((any Error)?) -> Void)

Inserts all tracks of an asset for a time range into a composition.

Deprecated

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime) throws

Inserts all the tracks within a given time range of a specified asset into the composition.

Deprecated

