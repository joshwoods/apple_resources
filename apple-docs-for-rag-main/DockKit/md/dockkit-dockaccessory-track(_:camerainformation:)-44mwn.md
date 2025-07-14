

- DockKit
- DockAccessory
-  track(\_:cameraInformation:) 

Instance Method

# track(\_:cameraInformation:)

Automatically generate and send tracking vectors to the device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.1+

``` source
final func track(
    _ data: [DockAccessory.Observation],
    cameraInformation: DockAccessory.CameraInformation
) async throws
```

## Parameters 

`data`  

An array of DockAccessory.Observation objects indicating the location of objects of interest in the frame.

`cameraInformation`  

The camera currently being used, and the orientation of the device.

## Discussion

The device receives tracking vectors based on manually constructed observations.

Disable system tracking, then supply the observations at a fixed rate between 10 and 30 times per second. Any other rate is unsupported. Calling this method without first disabling system tracking is a fatal error.

Throws

DockKitError.notSupported if called on macOS.

## See Also

### Selecting and tracking

func selectSubject(at: CGPoint) async throws

Selects a subject to track at the supplied coordinates.

func track([AVMetadataObject], cameraInformation: DockAccessory.CameraInformation) async throws

Automatically generate and send tracking vectors to the device.

struct Observation

An observation of the contents of a single video frame.

struct CameraInformation

A collection of tracking information about the camera currently in use.

enum CameraOrientation

The set of camera orientations used to extract coordinates.

