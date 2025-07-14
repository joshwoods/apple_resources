

- Synchronization
- Atomic
-  bitwiseAnd(\_:ordering:) 

Instance Method

# bitwiseAnd(\_:ordering:)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@discardableResult
func bitwiseAnd(
    _ operand: Int8,
    ordering: AtomicUpdateOrdering
) -> (oldValue: Int8, newValue: Int8)
```

Available when `Value` is `Int8`.

## Parameters 

`operand`  

An integer value.

`ordering`  

The memory ordering to apply on this operation.

## Return Value

A tuple containing the original value before the operation and the new value after the operation.

