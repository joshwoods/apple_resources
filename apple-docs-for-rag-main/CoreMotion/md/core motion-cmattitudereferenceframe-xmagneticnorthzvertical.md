

- Core Motion
- CMAttitudeReferenceFrame
-  xMagneticNorthZVertical 

Type Property

# xMagneticNorthZVertical

A reference frame where the Z axis is vertical and the X axis points to the magnetic north pole.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
static var xMagneticNorthZVertical: CMAttitudeReferenceFrame { get }
```

## Mentioned in 

Getting processed device-motion data

## Discussion

Use this option to determine the attitude of the device relative to magnetic north. For example, you might use this to implement a compass feature in your app. The yaw (Z-axis) value in CMAttitude is `0` when the X axis is aligned with magnetic north.

The device must have a magnetometer and that sensor must be available. If the magnetometer isn’t currently calibrated, Core Motion prompts the person to move the device to calibrate it.

## See Also

### Getting the reference frames

static var xArbitraryZVertical: CMAttitudeReferenceFrame

A reference frame where the Z axis is vertical and the X axis points in an arbitrary direction in the horizontal plane.

static var xArbitraryCorrectedZVertical: CMAttitudeReferenceFrame

A reference frame where the Z axis is vertical and has improved rotation accuracy, and the X axis points in an arbitrary direction in the horizontal plane.

static var xTrueNorthZVertical: CMAttitudeReferenceFrame

A reference frame where the Z axis is vertical and the X axis points to the geographic north pole.

