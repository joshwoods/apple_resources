

- RealityKit
- Entity
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Indicates whether two entities are equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
nonisolated
static func == (lhs: Entity, rhs: Entity) -> Bool
```

## Parameters 

`lhs`  

The first entity to compare.

`rhs`  

The second entity to compare.

## Return Value

A Boolean value set to `true` if the two entities are equal.

## See Also

### Comparing entities

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the entity by feeding them into the given hash function.

var hashValue: Int

The hash value.

