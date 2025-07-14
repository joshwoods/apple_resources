

- Spatial
- Volumetric
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the entity contains the specified volumetric entity.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func contains(_ other: Self) -> Bool
```

**Required**

## Parameters 

`other`  

The volumetric entity that the function compares against.

## See Also

### Instance methods

func contains(point: Point3D) -> Bool

Returns a Boolean value that indicates whether this volume contains the specified point.

**Required**

func contains(anyOf: [Point3D]) -> Bool

Returns a Boolean value that indicates whether this volume contains any of the specified points.

**Required**

func formIntersection(Self)

Sets the primitive to the intersection of itself and the specified primitive.

**Required** Default implementation provided.

func formUnion(Self)

Sets the primitive to the union of itself and the specified primitive.

**Required** Default implementation provided.

func intersection(Self) -> Self?

Returns the intersection of two volumetric entities.

**Required**

func union(Self) -> Self

Returns the smallest volumetric entity that contains the two source entities.

**Required**

