

- RealityKit
-  ObjectCapturePointCloudView 

Structure

# ObjectCapturePointCloudView

Renders the current state of the point cloud from an object capture session.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
struct ObjectCapturePointCloudView
```

## Overview

This view renders a 3D visualization of the current session’s point cloud. It includes a turntable gesture controller. This view allows the user to review the captured 3D model before finishing the capture and beginning object reconstruction.

## Topics

### Initializers

init(session: ObjectCaptureSession)

Creates an object capture view from an existing session using the current segment’s point cloud.

### Instance Properties

var body: some View

The content and behavior of the view.

### Instance Methods

func showShotLocations(Bool) -> ObjectCapturePointCloudView

Shows the locations where shots have been taken. Example: ObjectCapturePointCloudView(session: mySession) .showShotLocations()

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

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

class ObjectCaptureSession

A session object that monitors and controls image capture for photogrammetry.

