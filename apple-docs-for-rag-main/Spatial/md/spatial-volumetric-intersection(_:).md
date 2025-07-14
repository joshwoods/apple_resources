

- Spatial
- Volumetric
-  intersection(\_:) 

Instance Method

# intersection(\_:)

Returns the intersection of two volumetric entities.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func intersection(_ other: Self) -> Self?
```

**Required**

## Parameters 

`other`  

The volumetric entity that the function compares against.

## See Also

### Instance methods

func contains(Self) -> Bool

Returns a Boolean value that indicates whether the entity contains the specified volumetric entity.

**Required**

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

func union(Self) -> Self

Returns the smallest volumetric entity that contains the two source entities.

**Required**

