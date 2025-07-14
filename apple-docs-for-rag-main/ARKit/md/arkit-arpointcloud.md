

- ARKit
-  ARPointCloud 

Class

# ARPointCloud

A collection of points in the world coordinate space of the AR session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARPointCloud
```

## Overview

Use the ARFrame rawFeaturePoints property to obtain a point cloud representing intermediate results of the scene analysis ARKit uses to perform world tracking.

## Topics

### Identifying Feature Points

var points: [simd_float3]

The list of detected points.

var identifiers: [UInt64]

A list of unique identifiers corresponding to detected feature points.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Video Frame Analysis

Displaying a point cloud using scene depth

Present a visualization of the physical environment by placing points based a scene’s depth data.

Creating a fog effect using scene depth

Apply virtual fog to the physical environment.

class ARFrame

A video image captured as part of a session with position-tracking information.

class ARDepthData

An object that describes the distance to regions of the real world from the plane of the camera.

