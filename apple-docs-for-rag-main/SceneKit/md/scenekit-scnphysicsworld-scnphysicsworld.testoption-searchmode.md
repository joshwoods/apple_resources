

- SceneKit
- SCNPhysicsWorld
- SCNPhysicsWorld.TestOption
-  searchMode 

Type Property

# searchMode

The key for selecting the number and order of contacts to be tested.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let searchMode: SCNPhysicsWorld.TestOption
```

## Discussion

See `Physics Test Search Modes` for possible values. The default value is any.

This key applies only to ray and convex sweep tests.

## See Also

### Type Properties

static let backfaceCulling: SCNPhysicsWorld.TestOption

The key for choosing whether to ignore back-facing polygons in physics shapes when searching for contacts.

static let collisionBitMask: SCNPhysicsWorld.TestOption

The key for selecting which categories of physics bodies that SceneKit should test for contacts.

struct TestSearchMode

Options affecting how SceneKit searches for bodies in a collision, ray, or sweep test, used with the searchMode key.

