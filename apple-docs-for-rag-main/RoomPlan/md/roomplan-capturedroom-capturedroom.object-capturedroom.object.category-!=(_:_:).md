

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
- CapturedRoom.Object.Category
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Determines whether two object categories aren’t equal.

RoomPlanSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

The category argument on the left-hand side of the operator.

`rhs`  

The category argument on the right-hand side of the operator.

## Return Value

`true` if the object categories aren’t equal. Otherwise, returns `false`.

## See Also

### Comparing object categories

static func == (CapturedRoom.Object.Category, CapturedRoom.Object.Category) -> Bool

Determines whether two object categories are equal.

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

