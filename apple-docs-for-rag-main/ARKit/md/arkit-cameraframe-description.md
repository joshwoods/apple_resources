

- ARKit
- CameraFrame
-  description 

Instance Property

# description

A textual representation of this camera frame.

visionOS 2.0+

``` source
var description: String { get }
```

## See Also

### Getting camera frame information

var primarySample: CameraFrame.Sample

Gets the primary frame sample for a camera frame.

struct Sample

Information that describes a sample from a camera frame.

func sample(for: CameraFrameProvider.CameraPosition) -> CameraFrame.Sample?

Returns the camera frame sample for a given camera position.

