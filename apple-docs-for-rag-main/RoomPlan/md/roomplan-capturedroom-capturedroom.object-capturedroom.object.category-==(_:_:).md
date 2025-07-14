

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
- CapturedRoom.Object.Category
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Determines whether two object categories are equal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static func == (a: CapturedRoom.Object.Category, b: CapturedRoom.Object.Category) -> Bool
```

## Parameters 

`lhs`  

The category argument on the left-hand side of the operator.

`rhs`  

The category argument on the right-hand side of the operator.

## Return Value

`true` if the categories are equal. Otherwise, returns `false`.

## See Also

### Comparing object categories

static func != (Self, Self) -> Bool

Determines whether two object categories aren’t equal.

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

