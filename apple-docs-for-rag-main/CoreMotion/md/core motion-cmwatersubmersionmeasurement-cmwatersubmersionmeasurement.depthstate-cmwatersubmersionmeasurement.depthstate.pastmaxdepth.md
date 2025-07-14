

- Core Motion
- CMWaterSubmersionMeasurement
- CMWaterSubmersionMeasurement.DepthState
-  CMWaterSubmersionMeasurement.DepthState.pastMaxDepth 

Case

# CMWaterSubmersionMeasurement.DepthState.pastMaxDepth

The device has exceeded the maximum safe diving depth.

iOS 4.0+iPadOS 4.0+visionOS 1.0+watchOS 2.0+

``` source
case pastMaxDepth
```

## Discussion

The system sets the maximum depth based on the entitlement that your app uses, as shown in this table:

| Shallow Depth and Pressure entitlement        | 6 m  |
|-----------------------------------------------|------|
| Full Submerged Depth and Pressure entitlement | 40 m |

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

case sensorDepthError

An error with the depth sensor occurred.

case unknown

The device’s depth state is unknown.

