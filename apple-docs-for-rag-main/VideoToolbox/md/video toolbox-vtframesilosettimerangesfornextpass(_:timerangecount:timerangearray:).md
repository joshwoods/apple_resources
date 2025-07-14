

- Video Toolbox
-  VTFrameSiloSetTimeRangesForNextPass(\_:timeRangeCount:timeRangeArray:) 

Function

# VTFrameSiloSetTimeRangesForNextPass(\_:timeRangeCount:timeRangeArray:)

Begins a new pass of samples to be added to a frame silo object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTFrameSiloSetTimeRangesForNextPass(
    _ silo: VTFrameSilo,
    timeRangeCount: CMItemCount,
    timeRangeArray: UnsafePointer
) -> OSStatus
```

## Parameters 

`silo`  

The frame silo object.

`timeRangeCount`  

The count of time ranges in `timeRangeArray`.

`timeRangeArray`  

The array of `CMTimeRange` structs.

## Return Value

`kVTFrameSiloInvalidTimeRangeErr` if any time ranges are non-numeric, overlap, or are not in ascending order.

## Discussion

Previously added sample buffers with decode timestamps within the time ranges are deleted from the frame silo object.

Note

It’s not necessary to call this function before adding sample buffers for the first pass.

## See Also

### Configuring Frame Silos

func VTFrameSiloAddSampleBuffer(VTFrameSilo, sampleBuffer: CMSampleBuffer) -> OSStatus

Adds a sample buffer to a frame silo object.

func VTFrameSiloCallBlockForEachSampleBuffer(VTFrameSilo, in: CMTimeRange, handler: (CMSampleBuffer) -> OSStatus) -> OSStatus

Retrieves sample buffers from a frame silo object.

func VTFrameSiloCallFunctionForEachSampleBuffer(VTFrameSilo, in: CMTimeRange, refcon: UnsafeMutableRawPointer?, callback: (UnsafeMutableRawPointer?, CMSampleBuffer) -> OSStatus) -> OSStatus

Retrieves sample buffers from a frame silo object.

