

- RoomPlan
- CapturedRoom
- CapturedRoom.Error
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Determines whether two captured room errors are equal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static func == (a: CapturedRoom.Error, b: CapturedRoom.Error) -> Bool
```

## Parameters 

`lhs`  

The error argument on the left-hand side of the operator.

`rhs`  

The error argument on the right-hand side of the operator.

## Return Value

`true` if the errors are equal. Otherwise, returns `false`.

## See Also

### Comparing errors

static func != (Self, Self) -> Bool

Determines whether two captured room errors aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

