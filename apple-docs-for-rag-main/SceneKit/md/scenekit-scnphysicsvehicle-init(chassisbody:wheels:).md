

- SceneKit
- SCNPhysicsVehicle
-  init(chassisBody:wheels:) 

Initializer

# init(chassisBody:wheels:)

Creates a vehicle behavior.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    chassisBody: SCNPhysicsBody,
    wheels: [SCNPhysicsVehicleWheel]
)
```

## Parameters 

`chassisBody`  

A physics body to serve as the vehicle’s chassis.

`wheels`  

An array of SCNPhysicsVehicleWheel objects representing the vehicle’s wheels. A vehicle must have at least one wheel.

## Return Value

A new vehicle behavior.

## Discussion

Each object in the `wheels` array associates a node with the wheel to serve as its visual representation and defines properties for the wheel’s physical characteristics. Each wheel object must reference a unique node, which should be a child of the node containing the physics body used for the vehicle’s chassis. Typically, you load a node hierarchy representing the vehicle and all of its wheels from a scene file and then designate which nodes serve as the body and wheels.

For a behavior to take effect, you must add it to the physics simulation by calling the addBehavior(_:) method on your scene’s SCNPhysicsWorld object.

