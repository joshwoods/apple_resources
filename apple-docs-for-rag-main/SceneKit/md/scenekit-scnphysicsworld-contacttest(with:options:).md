

- SceneKit
- SCNPhysicsWorld
-  contactTest(with:options:) 

Instance Method

# contactTest(with:options:)

Checks for contacts between one physics body and any other bodies in the physics world.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func contactTest(
    with body: SCNPhysicsBody,
    options: [SCNPhysicsWorld.TestOption : Any]? = nil
) -> [SCNPhysicsContact]
```

## Parameters 

`body`  

The body to test for contact.

`options`  

A dictionary of options affecting the test, or `nil` to use default options. For applicable keys and the possible values, see `Physics Test Options Keys`.

## Return Value

An array of SCNPhysicsContact objects describing contacts between the specified body and any others, or `nil` if the body is not in contact with any other bodies.

## Discussion

SceneKit sends messages to the physics world’s contactdelegate object only when collisions occur between bodies whose collisionBitMask and categoryBitMask properties overlap, and only for collisions between certain types of bodies. (For details, see SCNPhysicsBodyType.) Use this method to directly test for all contacts between one body and any other bodies at a time of your choosing. For example, to implement a game with a “wall jump” effect, you could call this method when the player presses the jump button to see if the player character is in contact with any walls.

## See Also

### Detecting Contacts Between Physics Bodies

var contactDelegate: (any SCNPhysicsContactDelegate)?

A delegate that is called when two physics bodies come in contact with each other.

func contactTestBetween(SCNPhysicsBody, SCNPhysicsBody, options: [SCNPhysicsWorld.TestOption : Any]?) -> [SCNPhysicsContact]

Checks for contacts between two physics bodies.

