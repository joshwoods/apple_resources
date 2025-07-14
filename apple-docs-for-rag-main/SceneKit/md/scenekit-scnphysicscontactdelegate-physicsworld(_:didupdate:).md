

- SceneKit
- SCNPhysicsContactDelegate
-  physicsWorld(\_:didUpdate:) 

Instance Method

# physicsWorld(\_:didUpdate:)

Tells the delegate that new information is available about an ongoing contact.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
optional func physicsWorld(
    _ world: SCNPhysicsWorld,
    didUpdate contact: SCNPhysicsContact
)
```

## Parameters 

`world`  

The physics world that is processing the contact.

`contact`  

An object that describes the contact.

## Discussion

SceneKit calls this method on each step of the physics simulation (see the timeStep property) if information about the contact changes—for example, if two bodies are sliding against one another.

## See Also

### Responding to Contact Events

func physicsWorld(SCNPhysicsWorld, didBegin: SCNPhysicsContact)

Tells the delegate that two bodies have come into contact.

func physicsWorld(SCNPhysicsWorld, didEnd: SCNPhysicsContact)

Tells the delegate that a contact has ended.

