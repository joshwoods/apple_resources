

- Spatial
- Scalable3D
-  uniformlyScale(by:) 

Instance Method

# uniformlyScale(by:)

Uniformly scales the entity by the specified scalar value.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func uniformlyScale(by scale: Double)
```

**Required** Default implementation provided.

## Parameters 

`scale`  

The double-precision value that specifies the uniform scale.

## Default Implementations

### Scalable3D Implementations

func uniformlyScale(by: Double)

Uniformly scales the entity by the specified scalar value.

## See Also

### Instance methods

func scale(by: Size3D)

Scales the entity by the specified size.

**Required** Default implementation provided.

func scaleBy(x: Double, y: Double, z: Double)

Scales the entity by the specified values.

**Required** Default implementation provided.

func scaled(by: Size3D) -> Self

Returns the entity that results from scaling with the specified size.

**Required**

func scaledBy(x: Double, y: Double, z: Double) -> Self

Returns the entity that results from scaling with the specified values.

**Required**

func uniformlyScaled(by: Double) -> Self

Returns the entity that results from uniformly scaling with the specified scalar value.

**Required**

