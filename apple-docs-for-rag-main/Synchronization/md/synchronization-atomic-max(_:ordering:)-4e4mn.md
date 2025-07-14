

- Synchronization
- Atomic
-  max(\_:ordering:) 

Instance Method

# max(\_:ordering:)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@discardableResult
func max(
    _ operand: Int128,
    ordering: AtomicUpdateOrdering
) -> (oldValue: Int128, newValue: Int128)
```

Available when `Value` is `Int128`.

## Parameters 

`operand`  

An integer value.

`ordering`  

The memory ordering to apply on this operation.

## Return Value

A tuple containing the original value before the operation and the new value after the operation.

