

- AVFoundation
- AVMutableComposition
-  insertEmptyTimeRange(\_:) 

Instance Method

# insertEmptyTimeRange(\_:)

Adds or extends an empty time range within all tracks of the composition.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func insertEmptyTimeRange(_ timeRange: CMTimeRange)
```

## Parameters 

`timeRange`  

The empty time range to insert.

## Discussion

Inserting an empty time range pushes out existing content by the time range’s duration. Use this method to reserve a time range in the composition for a subsequently created track to present its media.

## See Also

### Managing Time Ranges

func removeTimeRange(CMTimeRange)

Removes a specified time range from all tracks of the composition.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of all tracks in a given time range.

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime, completionHandler: ((any Error)?) -> Void)

Inserts all tracks of an asset for a time range into a composition.

Deprecated

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime) throws

Inserts all the tracks within a given time range of a specified asset into the composition.

Deprecated

