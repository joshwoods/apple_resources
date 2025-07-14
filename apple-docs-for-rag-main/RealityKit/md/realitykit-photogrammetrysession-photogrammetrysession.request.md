

- RealityKit
- PhotogrammetrySession
-  PhotogrammetrySession.Request 

Enumeration

# PhotogrammetrySession.Request

An object that configures a photogrammetry session reconstruction request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum Request
```

## Mentioned in 

Creating 3D objects from photographs

## Overview

Create a PhotogrammetrySession.Request for each 3D object you want to construct from the same set of photographs. You might, for example, create a session with two requests, one to generate a low-resolution preview object in memory, and a second to generate a high-resolution final object saved to the file system.

Before creating an instance of this class, check isSupported to ensure object capture is available on the current device.

For more information on using PhotogrammetrySession, see Creating 3D objects from photographs.

## Topics

### Creating the request

init(modelFile: URL)

Creates an instance based on the contents of a USDZ file.

### Specifying the output

case modelFile(url: URL, detail: PhotogrammetrySession.Request.Detail, geometry: PhotogrammetrySession.Request.Geometry?)

An object-creation request saved to a USDZ file or a folder (for OBJ output).

case modelEntity(detail: PhotogrammetrySession.Request.Detail, geometry: PhotogrammetrySession.Request.Geometry?)

An object-creation request stored in-memory for immediate display.

case bounds

An object-creation request that returns a box the same size as the created model.

enum Detail

Supported levels of detail for a request.

### Comparing values

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (PhotogrammetrySession.Request, PhotogrammetrySession.Request) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Transforming the created model

struct Geometry

An object that holds a bounding box and transformation data for a request.

### Enumeration Cases

case pointCloud

The raw detected points from the pictures with no polygons connecting them.

case poses

Requests the estimated pose of the camera in each shot (relative to the common estimated coordinate system shared with the `.bounds` request).

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

