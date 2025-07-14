

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
- CapturedRoom.Surface.Edge
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Determines whether two surface edges are equal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static func == (a: CapturedRoom.Surface.Edge, b: CapturedRoom.Surface.Edge) -> Bool
```

## Parameters 

`lhs`  

The edge argument on the left-hand side of the operator.

`rhs`  

The edge argument on the right-hand side of the operator.

## Return Value

`true` if the surface edges are equal. Otherwise, returns `false`.

## See Also

### Comparing edges

static func != (Self, Self) -> Bool

Determines whether two surface edges aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

