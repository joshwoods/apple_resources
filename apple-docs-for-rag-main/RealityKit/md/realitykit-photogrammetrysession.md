

- RealityKit
-  PhotogrammetrySession 

Class

# PhotogrammetrySession

Manages the creation of a 3D model from a set of images.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class PhotogrammetrySession
```

## Mentioned in 

Creating 3D objects from photographs

## Overview

For more information on using PhotogrammetrySession, see Creating 3D objects from photographs.

## Topics

### Creating the session

convenience init(input: URL, configuration: PhotogrammetrySession.Configuration) throws

Creates a session from a specified directory of images.

convenience init&lt;S>(input: S, configuration: PhotogrammetrySession.Configuration) throws

Creates a session from a sequence of samples.

static var isSupported: Bool

Returns `true` if the current hardware supports Object Capture.

### Configuring the session

var configuration: PhotogrammetrySession.Configuration

Readonly property containing the session configuration set in the construction.

struct Configuration

The configuration parameters for a photogrammetry session.

### Monitoring the session

var activeRequests: [PhotogrammetrySession.Request]

The session’s active request objects.

var isProcessing: Bool

The session is actively processing requests.

var outputs: PhotogrammetrySession.Outputs

Returns the outputs message stream which can be asynchronously iterated on.

enum Output

Status updates on the object-creation process.

### Controlling object creation

func process(requests: [PhotogrammetrySession.Request]) throws

Starts processing of the provided processing `requests`. Messages begin to be produced to the `output` publisher.

func cancel()

Requests cancellation of any running requests.

### Creating requests

enum Request

An object that configures a photogrammetry session reconstruction request.

### Obtaining results

enum Result

An object that holds the created 3D object.

struct PointCloud

A sparse point cloud data structure output as the payload of a `.pointCloud` request. A point cloud is an array of `PointCloud.Point` instances.

enum Error

The errors that can occur during reconstruction in a photogrammetry session.

struct Pose

A 6DOF pose relative to the estimated coordinate system.

struct Poses

Once initial photogrammetric calculations are complete, a data structure mapping the sample ID (or index if a folder was used) to the 6DOF algorithmically estimated pose of that sample is returned.

### Structures

struct Limits

Data structure to observe hardware limits for reconstruction. Note that these are specific to the device on which the `PhotogrammetrySession` is run.

struct Outputs

An asynchronous sequence of session-related updates.

### Type Properties

static let limits: PhotogrammetrySession.Limits

Observer for the device-specific constant hardware limits for reconstruction.

### Default Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- Identifiable

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

struct PhotogrammetrySample

An object that represents one image and its corresponding metadata.

struct ObjectCaptureView

A view that guides a user through capturing images for object capture.

class ObjectCaptureSession

A session object that monitors and controls image capture for photogrammetry.

struct ObjectCapturePointCloudView

Renders the current state of the point cloud from an object capture session.

