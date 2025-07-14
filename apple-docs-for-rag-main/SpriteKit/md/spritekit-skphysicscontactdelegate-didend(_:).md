

- SpriteKit
- SKPhysicsContactDelegate
-  didEnd(\_:) 

Instance Method

# didEnd(\_:)

Called when the contact ends between two physics bodies.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
optional func didEnd(_ contact: SKPhysicsContact)
```

## Parameters 

`contact`  

An object that describes the contact.

## Discussion

The two physics bodies described in the contact parameter are not passed in a guaranteed order. The following code shows how you might respond to the end of a contact event to execute code if either physics body is owned by a node with the name `ground`.

Listing 1. Responding to a contact event

```
func didEnd(_ contact: SKPhysicsContact){
    if contact.bodyA.node?.name == "ground" || contact.bodyB.node?.name == "ground" {
        // execute code to respond to object hitting ground
    }
}
```

## See Also

### Responding to Contact Events

func didBegin(SKPhysicsContact)

Called when two bodies first contact each other.

