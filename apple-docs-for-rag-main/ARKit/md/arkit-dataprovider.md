

- ARKit
-  DataProvider 

Protocol

# DataProvider

A source of live data from ARKit.

visionOS 1.0+

``` source
protocol DataProvider : AnyObject, CustomStringConvertible, Sendable
```

## Overview

Most providers supply an asynchronous sequence of updated anchors for the provider’s data type. For example, a HandTrackingProvider instance’s anchorUpdates property gives updates over time for hand anchors.

## Topics

### Inspecting a data provider

var state: DataProviderState

The current status of data coming from this provider.

**Required**

### Inspecting a data provider type

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The kinds of authorization you need to use a particular data provider type.

**Required**

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports a particular provider type.

**Required**

## Relationships

### Inherits From

- CustomStringConvertible
- Sendable

### Conforming Types

- BarcodeDetectionProvider
- CameraFrameProvider
- EnvironmentLightEstimationProvider
- HandTrackingProvider
- ImageTrackingProvider
- ObjectTrackingProvider
- PlaneDetectionProvider
- RoomTrackingProvider
- SceneReconstructionProvider
- StereoPropertiesProvider
- WorldTrackingProvider

## See Also

### visionOS

Setting up access to ARKit data

Check whether your app can use ARKit and respect people’s privacy.

class ARKitSession

The main entry point for receiving data from ARKit.

protocol Anchor

The identity, location, and orientation of an object in world space.

ARKit in visionOS

Create immersive augmented reality experiences.

