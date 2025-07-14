

- AVFoundation
-  AVCapturePhotoOutputReadinessCoordinatorDelegate 

Protocol

# AVCapturePhotoOutputReadinessCoordinatorDelegate

A delegate protocol to receive updates about a photo output’s capture readiness.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
protocol AVCapturePhotoOutputReadinessCoordinatorDelegate : NSObjectProtocol
```

## Topics

### Monitoring capture readiness

func readinessCoordinator(AVCapturePhotoOutputReadinessCoordinator, captureReadinessDidChange: AVCapturePhotoOutput.CaptureReadiness)

Tells the delegate that the capture readiness state of a photo output changed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Photo capture

Capturing consistent color images

Add the power of a photography studio and lighting rig to your app with the new Constant Color API.

Capturing Still and Live Photos

Configure and capture single or multiple still images, Live Photos, and other forms of photography.

Capturing Photos in RAW and Apple ProRAW Formats

Support professional photography workflows by enabling minimally processed image capture in your camera app.

Supporting Continuity Camera in Your Mac App

Incorporate scanned documents and pictures from a user’s iPhone, iPad, or iPod touch into your Mac app using Continuity Camera.

class AVCapturePhoto

A container for image data from a photo capture output.

class AVCaptureDeferredPhotoProxy

A lightly-processed photo with data that the system may use to process and fetch a higher-resolution asset at a later time.

class AVCapturePhotoOutput

A capture output for still image, Live Photos, and other photography workflows.

protocol AVCapturePhotoCaptureDelegate

Methods for monitoring progress and receiving results from a photo capture output.

class AVCapturePhotoOutputReadinessCoordinator

An object that monitors changes to a photo output’s capture readiness.

class AVCaptureStillImageOutput

A capture output for capturing still photos.

Deprecated

