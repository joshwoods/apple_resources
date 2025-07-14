

- SceneKit
- SCNPhysicsWorld
- SCNPhysicsWorld.TestOption
-  backfaceCulling 

Type Property

# backfaceCulling

The key for choosing whether to ignore back-facing polygons in physics shapes when searching for contacts.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let backfaceCulling: SCNPhysicsWorld.TestOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. The default value is true, specifying that the search should only return contacts with the exterior surfaces of any physics shapes. Change the value to false to consider contacts with both interior and exterior surfaces.

This key applies only to ray and convex sweep tests, and only to physics shapes created using the concavePolyhedron option.

## See Also

### Type Properties

static let collisionBitMask: SCNPhysicsWorld.TestOption

The key for selecting which categories of physics bodies that SceneKit should test for contacts.

static let searchMode: SCNPhysicsWorld.TestOption

The key for selecting the number and order of contacts to be tested.

struct TestSearchMode

Options affecting how SceneKit searches for bodies in a collision, ray, or sweep test, used with the searchMode key.

