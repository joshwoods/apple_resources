

- Video Toolbox
-  VTFrameSiloGetProgressOfCurrentPass(\_:progressOut:) 

Function

# VTFrameSiloGetProgressOfCurrentPass(\_:progressOut:)

Gets the progress of the current pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTFrameSiloGetProgressOfCurrentPass(
    _ silo: VTFrameSilo,
    progressOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`silo`  

The frame silo object.

`progressOut`  

Upon return, contains the progress of the current pass.

## Return Value

`kVTFrameSiloInvalidTimeRangeErr` if any time ranges are non-numeric, overlap or are not in ascending order.

## Discussion

Calculates the current progress based on the most recent sample buffer added and the current pass time ranges.

## See Also

### Inspecting Frame Silos

func VTFrameSiloGetTypeID() -> CFTypeID

Retrieves the Core Foundation type identifier for the frame silo object.

