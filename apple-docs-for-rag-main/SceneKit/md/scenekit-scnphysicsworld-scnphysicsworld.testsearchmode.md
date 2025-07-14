

- SceneKit
- SCNPhysicsWorld
-  SCNPhysicsWorld.TestSearchMode 

Structure

# SCNPhysicsWorld.TestSearchMode

Options affecting how SceneKit searches for bodies in a collision, ray, or sweep test, used with the searchMode key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct TestSearchMode
```

## Topics

### Type Properties

static let all: SCNPhysicsWorld.TestSearchMode

Searches should return all contacts matching the search parameters.

static let any: SCNPhysicsWorld.TestSearchMode

Searches should return only the first contact found regardless of its position relative to the search parameters.

static let closest: SCNPhysicsWorld.TestSearchMode

Searches should return only the closest contact to the beginning of the search.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Type Properties

static let backfaceCulling: SCNPhysicsWorld.TestOption

The key for choosing whether to ignore back-facing polygons in physics shapes when searching for contacts.

static let collisionBitMask: SCNPhysicsWorld.TestOption

The key for selecting which categories of physics bodies that SceneKit should test for contacts.

static let searchMode: SCNPhysicsWorld.TestOption

The key for selecting the number and order of contacts to be tested.

