

- RealityKit
- RealityViewContentProtocol
-  add(\_:) 

Instance Method

# add(\_:)

Adds an entity to this content.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
func add(_ entity: Entity)
```

## See Also

### Managing view content

func remove(Entity)

Removes an entity from this content, if present.

associatedtype Entities : EntityCollection

The type of collection used for `entities`.

**Required**

var entities: Self.Entities

A collection of RealityKit entities that this view content renders within the scene.

**Required**

