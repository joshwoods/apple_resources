

- Video Toolbox
-  VTFrameSiloGetTypeID() 

Function

# VTFrameSiloGetTypeID()

Retrieves the Core Foundation type identifier for the frame silo object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTFrameSiloGetTypeID() -> CFTypeID
```

## Return Value

The `CFTypeID` of the frame silo object.

## See Also

### Inspecting Frame Silos

func VTFrameSiloGetProgressOfCurrentPass(VTFrameSilo, progressOut: UnsafeMutablePointer&lt;Float32>) -> OSStatus

Gets the progress of the current pass.

