

- AVFoundation
-  Capture setup 

API Collection

# Capture setup

Configure built-in cameras and microphones, and external capture devices, for media capture.

## Overview

The AVFoundation Capture subsystem provides a common high-level architecture for video, photo, and audio capture services in iOS and macOS. Use this system if you want to:

- Build a custom camera UI to integrate shooting photos or videos into your app’s user experience.

- Give users more direct control over photo and video capture, such as focus, exposure, and stabilization options.

- Produce different results than the system camera UI, such as RAW format photos, depth maps, or videos with custom timed metadata.

- Get live access to pixel or audio data streaming directly from a capture device.

Note

To instead let the user capture media with the system camera UI within your app, see UIImagePickerController.

The main parts of the capture architecture are sessions, inputs, and outputs: Capture sessions connect one or more inputs to one or more outputs. Inputs are sources of media, including capture devices like the cameras and microphones built into an iOS device or Mac. Outputs acquire media from inputs to produce useful data, such as movie files written to disk or raw pixel buffers available for live processing.

## Topics

### Essentials

Requesting authorization to capture and save media

Prompt the user to authorize access to the camera, microphone, and photo library.

### Capture sessions

Setting Up a Capture Session

Configure input devices, output media, preview views, and basic settings before capturing photos or video.

Accessing the camera while multitasking on iPad

Operate the camera in Split View, Slide Over, Picture in Picture, and Stage Manager modes.

AVCam: Building a camera app

Capture photos and record video using the front and rear iPhone and iPad cameras.

AVMultiCamPiP: Capturing from Multiple Cameras

Simultaneously record the output from the front and back cameras into a single movie file by using a multi-camera capture session.

AVCamBarcode: Detecting Barcodes and Faces

Identify machine readable codes or faces by using the camera.

class AVCaptureSession

An object that configures capture behavior and coordinates the flow of data from input devices to capture outputs.

class AVCaptureMultiCamSession

A capture session that supports simultaneous capture from multiple inputs of the same media type.

class AVCaptureInput

An abstract superclass for objects that provide input data to a capture session.

class AVCaptureOutput

An abstract superclass for objects that provide media output destinations for a capture session.

class AVCaptureConnection

An object that represents a connection from a capture input to a capture output.

### Capture devices

Choosing a Capture Device

Select the front or back camera, or use advanced features like the TrueDepth camera or dual camera.

class AVCaptureDevice

An object that represents a hardware or virtual capture device like a camera or microphone.

class AVCaptureDeviceInput

An object that provides media input from a capture device to a capture session.

class AVContinuityDevice

A class that represents a physical iOS device that’s nearby and can provide access to its cameras and microphones.

class AVExternalStorageDevice

Represents a physical external storage device that stores media assets.

class AVExternalStorageDeviceDiscoverySession

Informs your app when the external storage devices connect to and disconnect from the system.

### Capture preview

class AVCaptureVideoPreviewLayer

A Core Animation layer that displays video from a camera device.

class AVCaptureAudioPreviewOutput

A capture output that provides a preview of the captured audio.

### Continuity camera

Supporting Continuity Camera in your tvOS app

Capture high-quality photos, video, and audio in your Apple TV app by connecting an iPhone or iPad as a continuity device.

Supporting Continuity Camera in your macOS app

Enable high-quality photo and video capture by using an iPhone camera as an external capture device.

class AVCaptureDeskViewApplication

An object that programmatically presents Desk View.

### Capture controls

Enhancing your app experience with the Camera Control

Provide direct access to your camera app’s features to help people quickly capture the perfect shot.

class AVCaptureControl

An abstract base class for controls that interact with the camera system.

class AVCaptureSystemZoomSlider

A control that adjusts the video zoom factor of a capture device within the system-recommended range.

class AVCaptureSystemExposureBiasSlider

A control that adjusts the exposure bias of a capture device within the system-recommended range.

class AVCaptureSlider

A slider control that selects a value from a bounded range.

class AVCaptureIndexPicker

A control for selecting from a set of mutually exclusive values by index.

## See Also

### Capture

Photo capture

Capture high-quality still images, Live Photos, and supporting photo data.

Audio and video capture

Capture audio and video directly to media files, or capture streams of media for direct access to media sample buffers.

Additional data capture

Capture additional data including depth and metadata, and synchronize capture from multiple outputs.

