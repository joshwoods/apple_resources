

- SceneKit
- SCNPhysicsWorld
-  contactTestBetween(\_:\_:options:) 

Instance Method

# contactTestBetween(\_:\_:options:)

Checks for contacts between two physics bodies.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func contactTestBetween(
    _ bodyA: SCNPhysicsBody,
    _ bodyB: SCNPhysicsBody,
    options: [SCNPhysicsWorld.TestOption : Any]? = nil
) -> [SCNPhysicsContact]
```

## Parameters 

`bodyA`  

The first body (to test for contact with the second).

`bodyB`  

The second body (to test for contact with the first).

`options`  

A dictionary of options affecting the test, or `nil` to use default options. For applicable keys and the possible values, see `Physics Test Options Keys`.

## Return Value

An array of SCNPhysicsContact objects describing contacts between the two bodies, or `nil` if the bodies are not in contact.

## Discussion

SceneKit sends messages to the physics world’s contactDelegate object only when collisions occur between bodies whose collisionBitMask and categoryBitMask properties overlap, and only for collisions between certain types of bodies. (For details, see SCNPhysicsBodyType.) Use this method to directly test for contacts between any two bodies at a time of your choosing. For example, to implement a game where the player character can pick up an item, you might call this method when the player presses the “pick up” button to see if the player character is in contact with the item to be picked up.

## See Also

### Detecting Contacts Between Physics Bodies

var contactDelegate: (any SCNPhysicsContactDelegate)?

A delegate that is called when two physics bodies come in contact with each other.

func contactTest(with: SCNPhysicsBody, options: [SCNPhysicsWorld.TestOption : Any]?) -> [SCNPhysicsContact]

Checks for contacts between one physics body and any other bodies in the physics world.

