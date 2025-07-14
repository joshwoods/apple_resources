

- RealityKit
- CollisionFilter
-  init(group:mask:) 

Initializer

# init(group:mask:)

Creates a collision filter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
init(
    group: CollisionGroup,
    mask: CollisionGroup
)
```

## Parameters 

`group`  

The collision group identifier.

`mask`  

The collision mask defines what objects will collide with objects using this filter.

## Discussion

Collision filters are created for the collision group specified in the `group` parameter. The `mask` parameter defines which objects will collide with the objects that use this filter. Because CollisionGroup conforms to OptionSet, you can specify any combination of collision groups in the `mask` parameter by using the various OptionSet methods like union(_:), subtracting(_:), and intersection(_:). Entities from any group contained in `mask` will collide with entities using this filter, while those not contained by `mask` will not.

To combine multiple groups into a filter, use the union(_:) method, like this:

```
let groupA = CollisionGroup(rawValue: 1 

A common use case is to want entities to collide with everything except one group, or a few groups. In a game, for example, you might not want a player’s pieces to collide with their own pieces, or you might not want players on the same team to collide with each other. You can accomplish that by starting with the all property, subtracting the group or groups that you don’t want the entities using this filter to collide with, like this:

```
// Create a filter that collides with everything except B
let notGroupB = CollisionGroup.all.subtracting(groupB)
```

## See Also

### Creating a collision filter

static let `default`: CollisionFilter

The default collision filter.

static let sensor: CollisionFilter

A collision filter for an entity that collides with everything.

