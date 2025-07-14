

- SceneKit
- SCNPhysicsWorld
- SCNPhysicsWorld.TestOption
-  collisionBitMask 

Type Property

# collisionBitMask

The key for selecting which categories of physics bodies that SceneKit should test for contacts.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let collisionBitMask: SCNPhysicsWorld.TestOption
```

## Discussion

The value for this key is an NSNumber object containing an NSUInteger value. SceneKit tests for contacts only with physics bodies whose categoryBitMask property overlaps with this bit mask. The default value is all, specifying that searches should test all physics bodies regardless of their category.

## See Also

### Type Properties

static let backfaceCulling: SCNPhysicsWorld.TestOption

The key for choosing whether to ignore back-facing polygons in physics shapes when searching for contacts.

static let searchMode: SCNPhysicsWorld.TestOption

The key for selecting the number and order of contacts to be tested.

struct TestSearchMode

Options affecting how SceneKit searches for bodies in a collision, ray, or sweep test, used with the searchMode key.

