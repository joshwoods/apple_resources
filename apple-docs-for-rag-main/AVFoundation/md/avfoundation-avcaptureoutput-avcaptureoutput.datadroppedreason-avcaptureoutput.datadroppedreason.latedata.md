

- AVFoundation
- AVCaptureOutput
- AVCaptureOutput.DataDroppedReason
-  AVCaptureOutput.DataDroppedReason.lateData 

Case

# AVCaptureOutput.DataDroppedReason.lateData

The system dropped data because you’ve configured capture output to drop data when delegate queue is in a blocked state, and there’s data to deliver.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+visionOS 1.0+

``` source
case lateData
```

## Discussion

Use the alwaysDiscardsLateVideoFrames property of AVCaptureVideoDataOutput or the alwaysDiscardsLateDepthData property of AVCaptureDepthDataOutput to choose whether the capture output discards data.

## See Also

### Reasons

case none

The system didn’t drop data.

case outOfBuffers

The system dropped data because the capture output exhausted its internal pool of memory buffers.

case discontinuity

The system dropped data because the device providing data experienced a discontinuity, and the output lost an unknown number of data objects.

