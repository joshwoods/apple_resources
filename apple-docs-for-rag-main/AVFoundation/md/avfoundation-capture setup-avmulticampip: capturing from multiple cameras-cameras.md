

- AVFoundation
- Capture setup
-  AVMultiCamPiP: Capturing from Multiple Cameras 

Sample Code

# AVMultiCamPiP: Capturing from Multiple Cameras

Simultaneously record the output from the front and back cameras into a single movie file by using a multi-camera capture session.

Download

iOS 15.0+iPadOS 15.0+Xcode 16.0+

## Overview

Note

This sample code project is associated with WWDC 2019 session 225: Advances in Camera Capture &amp; Portrait Segmentation.

### Configure the Sample Code Project

You must run this sample code on one of these devices:

- An iPhone with an A12 or later processor

- An iPad Pro with an A12X or later processor

## See Also

### Capture sessions

Setting Up a Capture Session

Configure input devices, output media, preview views, and basic settings before capturing photos or video.

Accessing the camera while multitasking on iPad

Operate the camera in Split View, Slide Over, Picture in Picture, and Stage Manager modes.

AVCam: Building a camera app

Capture photos and record video using the front and rear iPhone and iPad cameras.

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

