

- RealityKit
- Entity
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the entity by feeding them into the given hash function.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
nonisolated
func hash(into hasher: inout Hasher)
```

## Parameters 

`hasher`  

The hash function to use when combining the components of the entity.

## See Also

### Comparing entities

static func == (Entity, Entity) -> Bool

Indicates whether two entities are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

var hashValue: Int

The hash value.

