

- RoomPlan
- RoomCaptureSession
- RoomCaptureSession.Instruction
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Determines whether two instructions are equal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
static func == (a: RoomCaptureSession.Instruction, b: RoomCaptureSession.Instruction) -> Bool
```

## Parameters 

`lhs`  

The instruction argument on the left-hand side of the operator.

`rhs`  

The instruction argument on the right-hand side of the operator.

## Return Value

`true` if the instructions are equal. Otherwise, returns `false`.

## See Also

### Comparing instructions

static func != (Self, Self) -> Bool

Determines whether two instructions aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

