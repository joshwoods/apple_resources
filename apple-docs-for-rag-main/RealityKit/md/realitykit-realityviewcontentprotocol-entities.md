

- RealityKit
- RealityViewContentProtocol
-  entities 

Instance Property

# entities

A collection of RealityKit entities that this view content renders within the scene.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var entities: Self.Entities { get nonmutating set }
```

**Required**

## See Also

### Managing view content

func add(Entity)

Adds an entity to this content.

func remove(Entity)

Removes an entity from this content, if present.

associatedtype Entities : EntityCollection

The type of collection used for `entities`.

**Required**

