

- Synchronization
- Atomic
-  add(\_:ordering:) 

Instance Method

# add(\_:ordering:)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@discardableResult
func add(
    _ operand: UInt128,
    ordering: AtomicUpdateOrdering
) -> (oldValue: UInt128, newValue: UInt128)
```

Available when `Value` is `UInt128`.

## Parameters 

`operand`  

An integer value.

`ordering`  

The memory ordering to apply on this operation.

## Return Value

A tuple containing the original value before the operation and the new value after the operation.

## Discussion

Note

This operation checks for overflow at runtime and will trap if an overflow does occur. In `-Ounchecked` builds, overflow checking is not performed.

