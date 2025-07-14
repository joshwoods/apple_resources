

- AVFoundation
-  AVCapturePhotoOutputReadinessCoordinator 

Class

# AVCapturePhotoOutputReadinessCoordinator

An object that monitors changes to a photo output’s capture readiness.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
class AVCapturePhotoOutputReadinessCoordinator
```

## Overview

Use this object to coordinate user interface updates on the main queue with a AVCapturePhotoOutput that runs on a background queue. Adopt the AVCapturePhotoOutputReadinessCoordinatorDelegate protocol in your app and set its implementation as the coordinator’s delegate object to receive callbacks as the associated photo output’s captureReadiness state changes.

You can track additional capture requests with this object by calling its startTrackingCaptureRequest(using:) method. You can use it to synchronously update shutter button availability and appearance and on the main thread while calling the photo output’s capturePhoto(with:delegate:) method asynchronously on a background queue.

## Topics

### Creating a coordinator

init(photoOutput: AVCapturePhotoOutput)

Creates an object that helps coordinate user interface changes with a photo output that runs on a background queue.

### Setting the delegate object

var delegate: (any AVCapturePhotoOutputReadinessCoordinatorDelegate)?

The coordinator’s delegate object.

### Performing tracking requests

func startTrackingCaptureRequest(using: AVCapturePhotoSettings)

Tracks a capture request that uses the specified photo settings.

func stopTrackingCaptureRequest(using: Int64)

Stop tracking the capture request represented by the specified photo setting’s unique identifier.

### Determining readiness for capture

var captureReadiness: AVCapturePhotoOutput.CaptureReadiness

A value that indicates whether the coordinator’s photo output is ready to respond to new capture requests in a timely manner.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
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

protocol AVCapturePhotoOutputReadinessCoordinatorDelegate

A delegate protocol to receive updates about a photo output’s capture readiness.

class AVCaptureStillImageOutput

A capture output for capturing still photos.

Deprecated

