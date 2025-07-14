

- AVFoundation
- Photo capture
-  Capturing consistent color images 

Sample Code

# Capturing consistent color images

Add the power of a photography studio and lighting rig to your app with the new Constant Color API.

Download

iOS 18.0+iPadOS 18.0+Xcode 16.0+

## Overview

Note

This sample code project is associated with WWDC24 session 10162: Capturing consistent color images.

### Configure the sample code project

Run this sample code on a device that provides the required flash module, such as the following:

- iPhone 14 or later

- iPhone 14 Pro or later

- iPad Pro 11-inch (M4) or later

- iPad Pro 13-inch (M4) or later

## See Also

### Photo capture

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

protocol AVCapturePhotoOutputReadinessCoordinatorDelegate

A delegate protocol to receive updates about a photo output’s capture readiness.

class AVCaptureStillImageOutput

A capture output for capturing still photos.

Deprecated

