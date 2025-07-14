

- ARKit
- CameraFrameProvider
-  cameraFrameUpdates(for:) 

Instance Method

# cameraFrameUpdates(for:)

Gets a sequence of camera frame updates for a given video format.

visionOS 2.0+

``` source
final func cameraFrameUpdates(for cameraVideoFormat: CameraVideoFormat) -> CameraFrameProvider.CameraFrameUpdates?
```

## Parameters 

`cameraVideoFormat`  

The camera video format to get updates for.

## Return Value

The sequence of camera frame updates. Returns `nil` if the provider wasn’t initialized with this format.

## See Also

### Getting camera frame updates

struct CameraFrameUpdates

A sequence of camera frames.

