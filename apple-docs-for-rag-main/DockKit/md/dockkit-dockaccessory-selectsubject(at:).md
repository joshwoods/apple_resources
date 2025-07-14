

- DockKit
- DockAccessory
-  selectSubject(at:) 

Instance Method

# selectSubject(at:)

Selects a subject to track at the supplied coordinates.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final func selectSubject(at unitPoint: CGPoint) async throws
```

## Discussion

There may be times when more than one subject is in a video frame. Use this method to track a specific subject within that frame by passing a location within the frame. The coordinates are relative to the top left of the video frame, and are values between `0` and `1`. If the framework doesn’t detect a subject at the passed coordinates, the method throws an error.

If you disable system tracking, this configuration change applies to any custom tracking for this dock accessory. The configuration applies to any camera stream the app has open if system tracking is enabled.

Call this method when implementing your own custom tracking behavior.

Throws

DockKitError.notConnected if device isn’t docked, or other errors if no subject is found at the position.

## See Also

### Selecting and tracking

func track([AVMetadataObject], cameraInformation: DockAccessory.CameraInformation) async throws

Automatically generate and send tracking vectors to the device.

func track([DockAccessory.Observation], cameraInformation: DockAccessory.CameraInformation) async throws

Automatically generate and send tracking vectors to the device.

struct Observation

An observation of the contents of a single video frame.

struct CameraInformation

A collection of tracking information about the camera currently in use.

enum CameraOrientation

The set of camera orientations used to extract coordinates.

