

- Core Motion
- CMWaterSubmersionMeasurement
- CMWaterSubmersionMeasurement.DepthState
-  CMWaterSubmersionMeasurement.DepthState.notSubmerged 

Case

# CMWaterSubmersionMeasurement.DepthState.notSubmerged

The device is not submerged in water.

iOS 4.0+iPadOS 4.0+visionOS 1.0+watchOS 2.0+

``` source
case notSubmerged
```

## See Also

### Depth states

case submergedShallow

The device is submerged, but less than 1 meter under water.

case submergedDeep

The device is submerged at least 1 meter under water.

case approachingMaxDepth

The device is approaching the maximum safe diving depth.

case pastMaxDepth

The device has exceeded the maximum safe diving depth.

case sensorDepthError

An error with the depth sensor occurred.

case unknown

The device’s depth state is unknown.

