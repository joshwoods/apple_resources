

- SceneKit
- SCNPhysicsVehicle
-  setSteeringAngle(\_:forWheelAt:) 

Instance Method

# setSteeringAngle(\_:forWheelAt:)

Pivots the specified wheel around its steering axis.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func setSteeringAngle(
    _ value: CGFloat,
    forWheelAt index: Int
)
```

## Parameters 

`value`  

The angle to set the wheel at relative to its steering axis, in radians.

`index`  

The index, in the vehicle’s wheels array, of the wheel to be pivoted.

## Discussion

Steering angles are relative to the wheel’s steeringAxis vector. With the default steering axis of `{0.0, -1.0, 0.0}`, a steering angle of `0.0` represents neutral steering, positive values steer the vehicle to the right, and negative values steer to the left.

## See Also

### Driving a Vehicle

func applyEngineForce(CGFloat, forWheelAt: Int)

Applies a force between the specified wheel and the ground under the vehicle.

func applyBrakingForce(CGFloat, forWheelAt: Int)

Applies a force between the specified wheel and the ground under the vehicle.

var speedInKilometersPerHour: CGFloat

The vehicle’s ground speed, in kilometers per hour.

