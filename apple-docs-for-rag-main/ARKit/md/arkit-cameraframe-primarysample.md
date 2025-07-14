

- ARKit
- CameraFrame
-  primarySample 

Instance Property

# primarySample

Gets the primary frame sample for a camera frame.

visionOS 2.0+

``` source
var primarySample: CameraFrame.Sample { get }
```

## See Also

### Getting camera frame information

struct Sample

Information that describes a sample from a camera frame.

func sample(for: CameraFrameProvider.CameraPosition) -> CameraFrame.Sample?

Returns the camera frame sample for a given camera position.

var description: String

A textual representation of this camera frame.

