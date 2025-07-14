

- SceneKit
- SCNPhysicsContactDelegate
-  physicsWorld(\_:didEnd:) 

Instance Method

# physicsWorld(\_:didEnd:)

Tells the delegate that a contact has ended.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
optional func physicsWorld(
    _ world: SCNPhysicsWorld,
    didEnd contact: SCNPhysicsContact
)
```

## Parameters 

`world`  

The physics world that is processing the contact.

`contact`  

An object that describes the contact.

## See Also

### Responding to Contact Events

func physicsWorld(SCNPhysicsWorld, didBegin: SCNPhysicsContact)

Tells the delegate that two bodies have come into contact.

func physicsWorld(SCNPhysicsWorld, didUpdate: SCNPhysicsContact)

Tells the delegate that new information is available about an ongoing contact.

