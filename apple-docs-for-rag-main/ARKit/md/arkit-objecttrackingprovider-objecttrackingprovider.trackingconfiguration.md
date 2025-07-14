

- ARKit
- ObjectTrackingProvider
-  ObjectTrackingProvider.TrackingConfiguration 

Structure

# ObjectTrackingProvider.TrackingConfiguration

Parameters for changing object-tracking behavior.

visionOS 2.0+

``` source
struct TrackingConfiguration
```

## Overview

Your app needs to include the Object-tracking parameter adjustment entitlement to modify the tracking configuration; otherwise, it has no effect.

## Topics

### Creating a tracking configuration

init()

Creates a tracking configuration.

### Inspecting a tracking configuration

var detectionRate: Float

The frequency at which object detection runs, in Hz.

var maximumInstancesPerReferenceObject: Int

The maximum number of instances of each reference object type to allow tracking at once.

var maximumTrackableInstances: Int

The total number of object instances that you can track at the same time.

var movingObjectTrackingRate: Float

The frequency at which object tracking runs for moving objects, in Hz.

var stationaryObjectTrackingRate: Float

The frequency at which object tracking runs for stationary objects, in Hz.

### Instance Properties

var description: String

A textual representation of this tracking configuration.

## Relationships

### Conforms To

- CustomStringConvertible

## See Also

### Configuring object-tracking

var trackingConfiguration: ObjectTrackingProvider.TrackingConfiguration

Returns the current parameters that are being used to configure object tracking.

