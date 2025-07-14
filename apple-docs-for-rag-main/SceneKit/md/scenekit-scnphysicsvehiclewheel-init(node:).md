

- SceneKit
- SCNPhysicsVehicleWheel
-  init(node:) 

Initializer

# init(node:)

Creates a wheel object.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(node: SCNNode)
```

## Parameters 

`node`  

The node whose contents provide the wheel’s visual representation.

## Return Value

A new wheel object.

## Discussion

The node representing a wheel must be a child of the node whose physics body serves as the chassis of the SCNPhysicsVehicle behavior the wheel is attached to. Each wheel object must reference a unique node. To use the wheel, add it to the vehicle behavior using the addWheel: method.

SceneKit uses the node’s bounding box to determine the wheel’s initial size, and it uses the node’s position to determine the where the wheel connects to the vehicle’s chassis. You can change attributes using the radius and connectionPosition properties.

