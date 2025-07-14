

- SceneKit
- SCNPhysicsWorld
- SCNPhysicsWorld.TestSearchMode
-  all 

Type Property

# all

Searches should return all contacts matching the search parameters.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let all: SCNPhysicsWorld.TestSearchMode
```

## See Also

### Type Properties

static let any: SCNPhysicsWorld.TestSearchMode

Searches should return only the first contact found regardless of its position relative to the search parameters.

static let closest: SCNPhysicsWorld.TestSearchMode

Searches should return only the closest contact to the beginning of the search.

