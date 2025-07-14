

- Spatial
- Translatable3D
-  translate(by:) Deprecated

Instance Method

# translate(by:)

Translates the entity by the specified size.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func translate(by size: Size3D)
```

**Required** Default implementations provided.

Deprecated

Use `Vector3D` variant.

## Parameters 

`size`  

The size structure that defines the translation.

## Default Implementations

### Translatable3D Implementations

func translate(by: Vector3D)

func translate(by: Size3D)

Translates the entity by the specified size.

## See Also

### Deprecated methods

func translated(by: Size3D) -> Self

Returns the entity that results from translating with the specified size.

**Required** Default implementation provided.

Deprecated

