

- RealityKit
-  ObjectCaptureSession 

Class

# ObjectCaptureSession

A session object that monitors and controls image capture for photogrammetry.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
class ObjectCaptureSession
```

## Overview

An ObjectCaptureSession is used together with an ObjectCaptureView to present a view that assists in capturing images of an object for reconstruction of a 3D model by using a PhotogrammetrySession.

A capture session contains functions for starting and advancing the capture session through a state machine that controls the image capture process. Your app can also observe several properties of the capture session to determine the current state of the capture process.

Once a session enters the `.completed` state, your app can transfer the images to a Mac or use them locally on the iOS device for use in object reconstruction using PhotogrammetrySession. Model reconstruction is a separate phase which this session does not directly monitor or control.

## Topics

### Creating a session

init()

Creates a new object capture session.

### Checking availability

static var isSupported: Bool

A Boolean that indicates whether the current device supports object capture sessions.

### Configuring a session

var feedback: Set&lt;ObjectCaptureSession.Feedback>

The current set of active `Feedback` states.

enum Feedback

Provides information about possible problems with the capture session.

var isPaused: Bool

A Boolean value that indicates if the capture session is paused.

var state: ObjectCaptureSession.CaptureState

The current state of the capture session.

var cameraTracking: ObjectCaptureSession.Tracking

The current state of ARKit camera tracking.

enum Tracking

A data structure that describes the current tracking state for the camera.

### Monitoring the session

enum CaptureState

State of the capture session.

enum Error

Errors associated with the top-level computation of this class.

### Controlling the session

func cancel()

Requests that the capture session be canceled.

func finish()

Requests that the capture session be stopped and all data saved.

func pause()

Pauses the automatic capture and other resource-intense algorithms.

func requestImageCapture()

Requests a manual image capture.

func resume()

Resumes object tracking algorithms after pause() is called.

func startCapturing()

Begins taking images for object capture.

### Structures

struct Configuration

The configuration options for the session which are passed into the `start(imagesDirectory:configuration:)` call.

struct Updates

Used to provide an `AsyncSequence` of change events for the observable properties.

### Instance Properties

var cameraTrackingUpdates: ObjectCaptureSession.Updates&lt;ObjectCaptureSession.Tracking>

The `Updates` `AsyncSequence` for the `cameraTracking` property.

var canRequestImageCapture: Bool

Will be `true` only when a call to requestImageCapture() is expected to be successful. It will be `false` when not in the `.capturing` state or if the session is too busy to currently process a new request. There is a period of time after requesting an image capture where this property will be `false` and a new call to requestImageCapture() will not produce a new image.

var canRequestImageCaptureUpdates: ObjectCaptureSession.Updates&lt;Bool>

The `Updates` `AsyncSequence` for the `canRequestImagecapture` property.

var configuration: ObjectCaptureSession.Configuration

The read-only `Configuration` used to start the capture session. The configuration can be set by passing it to the `start()` call and it remains immutable after the session is started successfully.

var feedbackUpdates: ObjectCaptureSession.Updates&lt;Set&lt;ObjectCaptureSession.Feedback>>

The `Updates` `AsyncSequence` for the `feedback` property.

var isAutoCaptureEnabled: Bool

Enables/disables auto-capture system. If disabled, only manually triggered shots are taken.

var isPausedUpdates: ObjectCaptureSession.Updates&lt;Bool>

The `Updates` `AsyncSequence` for the `isPaused` property.

var maximumNumberOfInputImages: Int

The maximum number of images that can be used for on-device reconstruction.

var numberOfShotsTaken: Int

The number of shots taken in the entire capture session so far, including both automatic capture and manual capture.

var numberOfShotsTakenUpdates: ObjectCaptureSession.Updates&lt;Int>

The `Updates` `AsyncSequence` for the `numberOfShotsTaken` property.

var shouldPlayHaptics: Bool

Enables/disables haptics on devices that support it.

var stateUpdates: ObjectCaptureSession.Updates&lt;ObjectCaptureSession.CaptureState>

The `Updates` `AsyncSequence` for the `state` property.

var userCompletedScanPass: Bool

This property starts out `false` at the start of a capture and will switch to `true` when the user has moved the device in a full circular scan pass around the bounding box of the target object and captured enough data to fill completely the capture dial.

var userCompletedScanPassUpdates: ObjectCaptureSession.Updates&lt;Bool>

The `Updates` `AsyncSequence` for the `userCompletedScanPass` property.

### Instance Methods

func beginNewScanPass()

Resets the state of the capture dial such that the user will need to perform another complete scan pass to fill it and generate a new event in the published property userCompletedScanPass.

func beginNewScanPassAfterFlip()

Starts the capturing of a new side of the object, to be called after the object is scanned one side and flipped.

func resetDetection() -> Bool

Moves the session state from `.detecting` back to `.ready` to reset the bounding box and prepare to select a new one with a new call to `startDetecting()`.

func start(imagesDirectory: URL, configuration: ObjectCaptureSession.Configuration)

Starts the session with the provided output image directory and optional checkpoint directory.

func startDetecting() -> Bool

Requests that the session should start detecting the object in the center of the camera.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- Identifiable
- Observable
- Sendable

## See Also

### Model creation

Capturing photographs for RealityKit Object Capture

Take high-quality images of objects to generate 3D models.

Creating 3D objects from photographs

Construct virtual objects to use in your AR experiences.

Scanning objects using Object Capture

Implement a full scanning workflow for capturing objects on iOS devices.

Building an object reconstruction app

Reconstruct objects from user-selected input images by using photogrammetry.

Creating a Photogrammetry Command-Line App

Generate 3D objects from images using RealityKit Object Capture.

Using object capture assets in RealityKit

Create a chess game using RealityKit and assets created using Object Capture.

class PhotogrammetrySession

Manages the creation of a 3D model from a set of images.

struct PhotogrammetrySample

An object that represents one image and its corresponding metadata.

struct ObjectCaptureView

A view that guides a user through capturing images for object capture.

struct ObjectCapturePointCloudView

Renders the current state of the point cloud from an object capture session.

