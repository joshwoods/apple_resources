

- RoomPlan
- RoomCaptureSession
- RoomCaptureSession.Instruction
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Determines whether two instructions aren’t equal.

RoomPlanSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

The instruction argument on the left-hand side of the operator.

`rhs`  

The instruction argument on the right-hand side of the operator.

## Return Value

`true` if the instructions aren’t equal. Otherwise, returns `false`.

## See Also

### Comparing instructions

static func == (RoomCaptureSession.Instruction, RoomCaptureSession.Instruction) -> Bool

Determines whether two instructions are equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

