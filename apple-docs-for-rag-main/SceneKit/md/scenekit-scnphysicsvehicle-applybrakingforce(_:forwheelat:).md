

- SceneKit
- SCNPhysicsVehicle
-  applyBrakingForce(\_:forWheelAt:) 

Instance Method

# applyBrakingForce(\_:forWheelAt:)

Applies a force between the specified wheel and the ground under the vehicle.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func applyBrakingForce(
    _ value: CGFloat,
    forWheelAt index: Int
)
```

## Parameters 

`value`  

The magnitude of the torque, in newton-meters.

`index`  

The index of the wheel applying the force.

## Discussion

Applying a braking force causes the wheel to slow down regardless of the direction it’s currently spinning in.

As with all physical quantities in SceneKit, you need not use realistic force measurements in your app—the effects of the physics simulation depend on the relative differences between forces, not on their absolute values. You may use whatever values produce the behavior or gameplay you’re looking for as long as you use them consistently.

Calling this method applies a braking force for one step (or frame) of the physics simulation. To continuously decelerate a vehicle, call this method again on subequent simulation steps (for example, from your scene renderer delegate’s renderer(_:updateAtTime:) method) until the vehicle stops or reaches your desired speed.

## See Also

### Driving a Vehicle

func applyEngineForce(CGFloat, forWheelAt: Int)

Applies a force between the specified wheel and the ground under the vehicle.

func setSteeringAngle(CGFloat, forWheelAt: Int)

Pivots the specified wheel around its steering axis.

var speedInKilometersPerHour: CGFloat

The vehicle’s ground speed, in kilometers per hour.

