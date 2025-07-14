

- Video Toolbox
-  VTFrameSiloAddSampleBuffer(\_:sampleBuffer:) 

Function

# VTFrameSiloAddSampleBuffer(\_:sampleBuffer:)

Adds a sample buffer to a frame silo object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTFrameSiloAddSampleBuffer(
    _ silo: VTFrameSilo,
    sampleBuffer: CMSampleBuffer
) -> OSStatus
```

## Parameters 

`silo`  

The frame silo object.

`sampleBuffer`  

The sample buffer to add to the frame silo.

## Return Value

`kVTFrameSiloInvalidTimeRangeErr` if an attempt is made to add a sample buffer with an inappropriate decode timestamp.

## Discussion

Within each pass, sample buffers must have strictly increasing decode timestamps. Passes after the first pass begin with a call to VTFrameSiloSetTimeRangesForNextPass(_:timeRangeCount:timeRangeArray:).

After a call to VTFrameSiloSetTimeRangesForNextPass(_:timeRangeCount:timeRangeArray:), sample buffer decode timestamps must also be within the stated time ranges. Note that time ranges are considered to contain their start times but not their end times.

## See Also

### Configuring Frame Silos

func VTFrameSiloSetTimeRangesForNextPass(VTFrameSilo, timeRangeCount: CMItemCount, timeRangeArray: UnsafePointer&lt;CMTimeRange>) -> OSStatus

Begins a new pass of samples to be added to a frame silo object.

func VTFrameSiloCallBlockForEachSampleBuffer(VTFrameSilo, in: CMTimeRange, handler: (CMSampleBuffer) -> OSStatus) -> OSStatus

Retrieves sample buffers from a frame silo object.

func VTFrameSiloCallFunctionForEachSampleBuffer(VTFrameSilo, in: CMTimeRange, refcon: UnsafeMutableRawPointer?, callback: (UnsafeMutableRawPointer?, CMSampleBuffer) -> OSStatus) -> OSStatus

Retrieves sample buffers from a frame silo object.

