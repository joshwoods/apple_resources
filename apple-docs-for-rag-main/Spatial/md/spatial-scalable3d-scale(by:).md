

- Spatial
- Scalable3D
-  scale(by:) 

Instance Method

# scale(by:)

Scales the entity by the specified size.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func scale(by size: Size3D)
```

**Required** Default implementation provided.

## Parameters 

`size`  

The size structure that defines the scale.

## Default Implementations

### Scalable3D Implementations

func scale(by: Size3D)

Scales the entity by the specified size.

## See Also

### Instance methods

func scaleBy(x: Double, y: Double, z: Double)

Scales the entity by the specified values.

**Required** Default implementation provided.

func scaled(by: Size3D) -> Self

Returns the entity that results from scaling with the specified size.

**Required**

func scaledBy(x: Double, y: Double, z: Double) -> Self

Returns the entity that results from scaling with the specified values.

**Required**

func uniformlyScale(by: Double)

Uniformly scales the entity by the specified scalar value.

**Required** Default implementation provided.

func uniformlyScaled(by: Double) -> Self

Returns the entity that results from uniformly scaling with the specified scalar value.

**Required**

