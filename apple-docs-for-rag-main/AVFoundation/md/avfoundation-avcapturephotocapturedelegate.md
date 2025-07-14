

- AVFoundation
-  AVCapturePhotoCaptureDelegate 

Protocol

# AVCapturePhotoCaptureDelegate

Methods for monitoring progress and receiving results from a photo capture output.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
protocol AVCapturePhotoCaptureDelegate : NSObjectProtocol
```

## Mentioned in 

Saving Captured Photos

Configuring Camera Capture to Collect a Portrait Effects Matte

## Overview

You implement methods in the AVCapturePhotoCaptureDelegate protocol to be notified of progress and results when capturing photos with the AVCapturePhotoOutput class.

To capture a photo, you pass an object implementing this protocol to the capturePhoto(with:delegate:) method, along with a settings object that describes the capture to be performed. As the capture proceeds, the photo output calls several of the methods in this protocol on your delegate object, providing information about the capture’s progress and delivering the resulting photos.

Which delegate methods the photo output calls depends on the photo settings you initiate capture with. All methods in this protocol are optional at compile time, but at run time your delegate object must respond to certain methods depending on your photo settings:

- If you request a still photo capture (by specifying image formats or file types), your delegate either must implement the photoOutput(_:didFinishProcessingPhoto:error:) method, or must implement methods listed in `Receiving Capture Results (Deprecated)` corresponding to whether you request capture in RAW format, processed format, or both.

- If you request Live Photo capture (by setting the livePhotoMovieFileURL property to a non-`nil` value), your delegate must implement the photoOutput(_:didFinishProcessingLivePhotoToMovieFileAt:duration:photoDisplayTime:resolvedSettings:error:) method.

The capture output validates these requirements when you call the capturePhoto(with:delegate:) method. If your delegate does not meet these requirements, that method raises an exception.

You must use a unique AVCapturePhotoSettings object for each capture request. When the photo output calls your delegate methods, it provides an AVCaptureResolvedPhotoSettings object whose uniqueID property matches that of the photo settings you requested capture with. When making multiple captures, use this unique ID to determine which delegate method calls correspond to which requests.

The photo output always calls each method listed in Monitoring Capture Progress exactly once for each capture request. For methods listed in Receiving Capture Results, you may receive a call more than once, or not at all, depending on your photo settings. See the description of each method for details.

## Topics

### Monitoring Capture Progress

func photoOutput(AVCapturePhotoOutput, willBeginCaptureFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the capture output has resolved settings and will soon begin its capture process.

func photoOutput(AVCapturePhotoOutput, willCapturePhotoFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that photo capture is about to occur.

func photoOutput(AVCapturePhotoOutput, didCapturePhotoFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the photo has been taken.

func photoOutput(AVCapturePhotoOutput, didFinishCaptureFor: AVCaptureResolvedPhotoSettings, error: (any Error)?)

Notifies the delegate that the capture process is complete.

### Receiving Capture Results

func photoOutput(AVCapturePhotoOutput, didFinishProcessingPhoto: AVCapturePhoto, error: (any Error)?)

Provides the delegate with the captured image and associated metadata resulting from a photo capture.

func photoOutput(AVCapturePhotoOutput, didFinishRecordingLivePhotoMovieForEventualFileAt: URL, resolvedSettings: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the movie content of a Live Photo has finished recording.

func photoOutput(AVCapturePhotoOutput, didFinishProcessingLivePhotoToMovieFileAt: URL, duration: CMTime, photoDisplayTime: CMTime, resolvedSettings: AVCaptureResolvedPhotoSettings, error: (any Error)?)

Provides the delegate the movie file URL resulting from a Live Photo capture.

func photoOutput(AVCapturePhotoOutput, didFinishCapturingDeferredPhotoProxy: AVCaptureDeferredPhotoProxy?, error: (any Error)?)

Tells the delegate when the system finishes capturing the photo proxy.

func photoOutput(AVCapturePhotoOutput, didFinishProcessingPhoto: CMSampleBuffer?, previewPhoto: CMSampleBuffer?, resolvedSettings: AVCaptureResolvedPhotoSettings, bracketSettings: AVCaptureBracketedStillImageSettings?, error: (any Error)?)

Provides the delegate a captured image in a processed format (such as JPEG).

Deprecated

func photoOutput(AVCapturePhotoOutput, didFinishProcessingRawPhoto: CMSampleBuffer?, previewPhoto: CMSampleBuffer?, resolvedSettings: AVCaptureResolvedPhotoSettings, bracketSettings: AVCaptureBracketedStillImageSettings?, error: (any Error)?)

Provides the delegate a captured image in RAW format.

Deprecated

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

class AVCapturePhotoOutputReadinessCoordinator

An object that monitors changes to a photo output’s capture readiness.

protocol AVCapturePhotoOutputReadinessCoordinatorDelegate

A delegate protocol to receive updates about a photo output’s capture readiness.

class AVCaptureStillImageOutput

A capture output for capturing still photos.

Deprecated

