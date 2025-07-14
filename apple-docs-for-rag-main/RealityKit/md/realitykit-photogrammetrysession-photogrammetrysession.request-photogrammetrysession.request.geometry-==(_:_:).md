

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
- PhotogrammetrySession.Request.Geometry
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
static func == (a: PhotogrammetrySession.Request.Geometry, b: PhotogrammetrySession.Request.Geometry) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## See Also

### Comparing geometry values

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

