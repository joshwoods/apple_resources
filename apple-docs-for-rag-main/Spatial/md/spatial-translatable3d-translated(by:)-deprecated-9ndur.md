

- Spatial
- Translatable3D
-  translated(by:) Deprecated

Instance Method

# translated(by:)

Returns the entity that results from translating with the specified size.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func translated(by size: Size3D) -> Self
```

**Required** Default implementation provided.

Deprecated

Use `Vector3D` variant.

## Parameters 

`size`  

The size structure that defines the translation.

## Default Implementations

### Translatable3D Implementations

func translated(by: Vector3D) -> Self

## See Also

### Deprecated methods

func translate(by: Size3D)

Translates the entity by the specified size.

**Required** Default implementations provided.

Deprecated

