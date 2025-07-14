

- SpriteKit
- SKPhysicsBody
-  init(bodies:) 

Initializer

# init(bodies:)

Creates a physics body that’s shaped like a union of the argument physics bodies.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(bodies: [SKPhysicsBody])
```

## Parameters 

`bodies`  

An array of SKPhysicsBody objects. The objects must be volume-based physics bodies. (You may not use a compound body created using this method in the array.)

## Return Value

A new compound-physics body.

## Discussion

The shapes of the physics bodies passed into this method are used to create a new physics body whose covered area is the union of the areas of its children. These areas do not need to be contiguous. If there is space between two parts, other bodies may be able to pass between these parts. However, the physics body is treated as a single connected body, meaning that a force or impulse applied to the body affects all of the pieces as if they are held together with an indestructible frame.

The properties on the children, such as mass or friction, are ignored. Only the shapes of the child bodies are used.

