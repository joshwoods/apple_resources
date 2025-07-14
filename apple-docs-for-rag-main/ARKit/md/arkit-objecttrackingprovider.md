

- ARKit
-  ObjectTrackingProvider 

Class

# ObjectTrackingProvider

A source of real-time position of reference objects in a person’s environment.

visionOS 2.0+

``` source
final class ObjectTrackingProvider
```

## Overview

Use this class to configure ARKIt to track reference objects in a person’s environment and receive a stream of updates that contains ObjectAnchor structures that describe them.

## Topics

### Creating an object-tracking provider

init(referenceObjects: [ReferenceObject], trackingConfiguration: ObjectTrackingProvider.TrackingConfiguration?)

Creates an object-tracking provider.

### Checking availability

static var isSupported: Bool

A Boolean value that indicates whether a device supports the object-tracking provider.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

An array of authorization types the object-tracking provider requires.

### Configuring object-tracking

var trackingConfiguration: ObjectTrackingProvider.TrackingConfiguration

Returns the current parameters that are being used to configure object tracking.

struct TrackingConfiguration

Parameters for changing object-tracking behavior.

### Inspecting an object-tracking provider

var state: DataProviderState

The state of an object-tracking provider.

var allAnchors: [ObjectAnchor]

An array of all the object anchors the object-tracking provider is tracking.

var anchorUpdates: AnchorUpdateSequence&lt;ObjectAnchor>

An asynchronous sequence of anchors the framework updates.

struct Error

Values that represent an object-tracking error.

var description: String

A textual representation of this object tracking provider.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### Object tracking

struct ObjectAnchor

A reference object ARKit is tracking.

Exploring object tracking with ARKit

Find and track real-world objects in visionOS using reference objects trained with Create ML.

Implementing object tracking in your visionOS app

Create engaging interactions by training models to recognize and track real-world objects in your app.

