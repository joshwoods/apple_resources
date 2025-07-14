

- RoomPlan
- CapturedRoom
- CapturedRoom.Confidence
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Determines whether two confidence values aren’t equal.

RoomPlanSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

The confidence argument on the left-hand side of the operator.

`rhs`  

The confidence argument on the right-hand side of the operator.

## Return Value

`true` if the confidence values aren’t equal. Otherwise, returns `false`.

## See Also

### Comparing confidence values

static func == (CapturedRoom.Confidence, CapturedRoom.Confidence) -> Bool

Determines whether two confidence values are equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

