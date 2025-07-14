

- SceneKit
- SCNPhysicsContactDelegate
-  physicsWorld(\_:didBegin:) 

Instance Method

# physicsWorld(\_:didBegin:)

Tells the delegate that two bodies have come into contact.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
optional func physicsWorld(
    _ world: SCNPhysicsWorld,
    didBegin contact: SCNPhysicsContact
)
```

## Parameters 

`world`  

The physics world that is processing the contact.

`contact`  

An object that describes the contact.

## See Also

### Responding to Contact Events

func physicsWorld(SCNPhysicsWorld, didUpdate: SCNPhysicsContact)

Tells the delegate that new information is available about an ongoing contact.

func physicsWorld(SCNPhysicsWorld, didEnd: SCNPhysicsContact)

Tells the delegate that a contact has ended.

