

- SceneKit
- SCNPhysicsVehicle
-  speedInKilometersPerHour 

Instance Property

# speedInKilometersPerHour

The vehicle’s ground speed, in kilometers per hour.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var speedInKilometersPerHour: CGFloat { get }
```

## See Also

### Driving a Vehicle

func applyEngineForce(CGFloat, forWheelAt: Int)

Applies a force between the specified wheel and the ground under the vehicle.

func applyBrakingForce(CGFloat, forWheelAt: Int)

Applies a force between the specified wheel and the ground under the vehicle.

func setSteeringAngle(CGFloat, forWheelAt: Int)

Pivots the specified wheel around its steering axis.

