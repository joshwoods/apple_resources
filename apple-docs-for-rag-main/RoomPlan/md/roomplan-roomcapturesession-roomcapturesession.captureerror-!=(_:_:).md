

- RoomPlan
- RoomCaptureSession
- RoomCaptureSession.CaptureError
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Determines whether two errors aren’t equal.

RoomPlanSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

The error argument on the left-hand side of the operator.

`rhs`  

The error argument on the right-hand side of the operator.

## Return Value

`true` if the errors aren’t equal. Otherwise, returns `false`.

## See Also

### Comparing errors

static func == (RoomCaptureSession.CaptureError, RoomCaptureSession.CaptureError) -> Bool

Determines whether two errors are equal.

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

