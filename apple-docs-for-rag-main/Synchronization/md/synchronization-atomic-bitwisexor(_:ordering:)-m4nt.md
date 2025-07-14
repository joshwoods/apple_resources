

- Synchronization
- Atomic
-  bitwiseXor(\_:ordering:) 

Instance Method

# bitwiseXor(\_:ordering:)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@discardableResult
func bitwiseXor(
    _ operand: UInt8,
    ordering: AtomicUpdateOrdering
) -> (oldValue: UInt8, newValue: UInt8)
```

Available when `Value` is `UInt8`.

## Parameters 

`operand`  

An integer value.

`ordering`  

The memory ordering to apply on this operation.

## Return Value

A tuple containing the original value before the operation and the new value after the operation.

