

- Spatial
- Scalable3D
-  scaleBy(x:y:z:) 

Instance Method

# scaleBy(x:y:z:)

Scales the entity by the specified values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func scaleBy(
    x: Double,
    y: Double,
    z: Double
)
```

**Required** Default implementation provided.

## Parameters 

`x`  

The double-precision value that specifies the scale along the x-dimension.

`y`  

The double-precision value that specifies the scale along the y-dimension.

`z`  

The double-precision value that specifies the scale along the z-dimension.

## Default Implementations

### Scalable3D Implementations

func scaleBy(x: Double, y: Double, z: Double)

Scales the entity by the specified values.

## See Also

### Instance methods

func scale(by: Size3D)

Scales the entity by the specified size.

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

