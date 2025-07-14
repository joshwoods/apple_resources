

- Spatial
- Translatable3D
-  translate(by:) 

Instance Method

# translate(by:)

Translates the entity by the specified vector.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func translate(by vector: Vector3D)
```

**Required** Default implementations provided.

## Parameters 

`vector`  

The vector that defines the translation.

## Default Implementations

### Translatable3D Implementations

func translate(by: Size3D)

Translates the entity by the specified size.

Deprecated

func translate(by: Vector3D)

## See Also

### Instance methods

func translated(by: Vector3D) -> Self

Returns the entity that results from translating with the specified vector.

**Required** Default implementation provided.

