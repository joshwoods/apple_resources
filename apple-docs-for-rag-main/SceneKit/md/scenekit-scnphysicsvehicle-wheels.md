

- SceneKit
- SCNPhysicsVehicle
-  wheels 

Instance Property

# wheels

An array of SCNPhysicsVehicleWheel objects representing the vehicle’s wheels.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var wheels: [SCNPhysicsVehicleWheel] { get }
```

## Discussion

You can dynamically change the suspension and traction properties of a wheel connected to the vehicle by using the corresponding SCNPhysicsVehicleWheel object or by using Key-value coding with a keypath of the form `wheels[index].propertyName`. For example, the following code changes the size of the first wheel attached to the vehicle, simulating a failed tire:

```
SCNPhysicsVehicle *vehicle = [SCNPhysicsVehicle vehicleWithChassisBody:car wheels:wheels];
[vehicle setValue:@0.1 forKeyPath:@"wheels[0].radius"];
```

## See Also

### Working with a Vehicle’s Physical Characteristics

var chassisBody: SCNPhysicsBody

The physics body representing the vehicle’s chassis.

