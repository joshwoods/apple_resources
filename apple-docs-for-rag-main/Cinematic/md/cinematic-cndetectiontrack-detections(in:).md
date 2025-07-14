

- Cinematic
- CNDetectionTrack
-  detections(in:) 

Instance Method

# detections(in:)

Returns the array of detections in the detection track within the given time range.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
func detections(in timeRange: CMTimeRange) -> [CNDetection]
```

## Parameters 

`timeRange`  

The time range of interest.

## Return Value

The array of detections in the detection track within the given time range. The return value is only appropriate for discrete detection tracks.

