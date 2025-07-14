

- ARKit
- CameraFrame
-  sample(for:) 

Instance Method

# sample(for:)

Returns the camera frame sample for a given camera position.

visionOS 2.0+

``` source
func sample(for position: CameraFrameProvider.CameraPosition) -> CameraFrame.Sample?
```

## Parameters 

`position`  

The camera position to get the sample for.

## Return Value

The camera frame sample, or `nil` if no sample is available for the given camera position.

## See Also

### Getting camera frame information

var primarySample: CameraFrame.Sample

Gets the primary frame sample for a camera frame.

struct Sample

Information that describes a sample from a camera frame.

var description: String

A textual representation of this camera frame.

