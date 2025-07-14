

- ARKit
-  ARTrackedRaycast 

Class

# ARTrackedRaycast

A raycast query that ARKit repeats in succession to give you refined results over time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARTrackedRaycast
```

## Overview

Tracked raycasting improves hit-testing techniques by repeating the query for a 3D position in succession. ARKit provides you with an updated position as it refines its understanding of world over time.

To start a tracked raycast, you call trackedRaycast(_:updateHandler:) on your app’s current ARSession.

## Topics

### Stopping Tracking

func stopTracking()

Stops repeating the raycast query.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Raycasting

Placing objects and handling 3D interaction

Place virtual content at tracked, real-world locations, and enable the user to interact with virtual content by using gestures.

class ARRaycastQuery

A mathematical ray you use to find 3D positions on real-world surfaces.

class ARRaycastResult

Information about a real-world surface found by examining a point on the screen.

