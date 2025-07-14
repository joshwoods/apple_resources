

- Cinematic
- CNDetectionTrack
-  detection(nearest:) 

Instance Method

# detection(nearest:)

Returns the array of detections in the detection track nearest a given time.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
func detection(nearest time: CMTime) -> CNDetection?
```

## Parameters 

`time`  

The time.

## Return Value

A number representing a properly time-stamped detection. The return value is only appropriate for discrete detection tracks.

