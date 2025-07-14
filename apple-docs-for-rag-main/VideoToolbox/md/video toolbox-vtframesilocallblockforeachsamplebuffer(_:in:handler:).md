

- Video Toolbox
-  VTFrameSiloCallBlockForEachSampleBuffer(\_:in:handler:) 

Function

# VTFrameSiloCallBlockForEachSampleBuffer(\_:in:handler:)

Retrieves sample buffers from a frame silo object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTFrameSiloCallBlockForEachSampleBuffer(
    _ silo: VTFrameSilo,
    in timeRange: CMTimeRange,
    handler: (CMSampleBuffer) -> OSStatus
) -> OSStatus
```

## Parameters 

`silo`  

The frame silo object.

`timeRange`  

The decode time range of sample buffers to retrieve. Pass `kCMTimeRangeInvalid` to retrieve all sample buffers from the `VTFrameSilo`.

`handler`  

A block to be called, in decode order, with each sample buffer that was added. To abort iteration early, return a nonzero status. The `VTFrameSilo` object may write sample buffers and data to the backing file between addition and retrieval; do not expect to get identical object pointers back.

## Return Value

`kVTFrameSiloInvalidTimeRangeErr` if any time ranges are non-numeric, overlap, or are not in ascending order. Returns any nonzero status returned by the handler block.

## Discussion

You call this function to retrieve sample buffers at the end of a multipass compression session.

## See Also

### Configuring Frame Silos

func VTFrameSiloAddSampleBuffer(VTFrameSilo, sampleBuffer: CMSampleBuffer) -> OSStatus

Adds a sample buffer to a frame silo object.

func VTFrameSiloSetTimeRangesForNextPass(VTFrameSilo, timeRangeCount: CMItemCount, timeRangeArray: UnsafePointer&lt;CMTimeRange>) -> OSStatus

Begins a new pass of samples to be added to a frame silo object.

func VTFrameSiloCallFunctionForEachSampleBuffer(VTFrameSilo, in: CMTimeRange, refcon: UnsafeMutableRawPointer?, callback: (UnsafeMutableRawPointer?, CMSampleBuffer) -> OSStatus) -> OSStatus

Retrieves sample buffers from a frame silo object.

