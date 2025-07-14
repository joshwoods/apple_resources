

- RealityKit
- Object capture
-  Building an object reconstruction app 

Sample Code

# Building an object reconstruction app

Reconstruct objects from user-selected input images by using photogrammetry.

Download

macOS 15.0+Xcode 16.0+

## Overview

Note

This sample code project is associated with WWDC24 session 10107: Discover Area Mode for Object Capture.

## See Also

### Model creation

Capturing photographs for RealityKit Object Capture

Take high-quality images of objects to generate 3D models.

Creating 3D objects from photographs

Construct virtual objects to use in your AR experiences.

Scanning objects using Object Capture

Implement a full scanning workflow for capturing objects on iOS devices.

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

class ObjectCaptureSession

A session object that monitors and controls image capture for photogrammetry.

struct ObjectCapturePointCloudView

Renders the current state of the point cloud from an object capture session.

