

- Spatial
- Shearable3D
-  shear(\_:) 

Instance Method

# shear(\_:)

Shears the entity by the specified axis and shear factors.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func shear(_ shear: AxisWithFactors)
```

**Required** Default implementation provided.

## Parameters 

`shear`  

The shear axis and factors.

## Default Implementations

### Shearable3D Implementations

func shear(AxisWithFactors)

Shears the entity by the specified axis and shear factors.

## See Also

### Instance methods

func sheared(AxisWithFactors) -> Self

Returns the entity that results from shearing with the specified axis and shear factors.

**Required**

