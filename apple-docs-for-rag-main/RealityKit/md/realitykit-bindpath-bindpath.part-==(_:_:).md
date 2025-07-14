

- RealityKit
- BindPath
- BindPath.Part
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two components of a bind path are equal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static func == (lhs: BindPath.Part, rhs: BindPath.Part) -> Bool
```

## Parameters 

`lhs`  

The component of the bind path on the left side of the operator.

`rhs`  

The component of the bind path on the right side of the operator.

## Return Value

Returns `true` if the components of the bind path are equal. Otherwise, returns `false`.

## See Also

### Comparing bind parts

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

