

- Core Motion
- CMWaterSubmersionMeasurement
- CMWaterSubmersionMeasurement.DepthState
-  CMWaterSubmersionMeasurement.DepthState.unknown 

Case

# CMWaterSubmersionMeasurement.DepthState.unknown

The device’s depth state is unknown.

iOS 4.0+iPadOS 4.0+visionOS 1.0+watchOS 2.0+

``` source
case unknown
```

## See Also

### Depth states

case notSubmerged

The device is not submerged in water.

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

