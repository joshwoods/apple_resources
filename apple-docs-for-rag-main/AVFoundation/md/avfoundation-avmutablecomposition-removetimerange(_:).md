

- AVFoundation
- AVMutableComposition
-  removeTimeRange(\_:) 

Instance Method

# removeTimeRange(\_:)

Removes a specified time range from all tracks of the composition.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func removeTimeRange(_ timeRange: CMTimeRange)
```

## Parameters 

`timeRange`  

The time range to remove.

## Discussion

After removing, existing content after the time range moves forward in the composition timeline.

Removing a time range doesn’t remove any existing tracks from the composition, even if removing it results in an empty track. Instead, it removes or truncates track segments that intersect with the time range.

## See Also

### Managing Time Ranges

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of all tracks in a given time range.

func insertEmptyTimeRange(CMTimeRange)

Adds or extends an empty time range within all tracks of the composition.

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime, completionHandler: ((any Error)?) -> Void)

Inserts all tracks of an asset for a time range into a composition.

Deprecated

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime) throws

Inserts all the tracks within a given time range of a specified asset into the composition.

Deprecated

