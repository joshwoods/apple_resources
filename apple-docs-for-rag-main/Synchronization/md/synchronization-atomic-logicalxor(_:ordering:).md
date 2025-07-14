

- Synchronization
- Atomic
-  logicalXor(\_:ordering:) 

Instance Method

# logicalXor(\_:ordering:)

Perform an atomic logical XOR operation and return the old and new value, applying the specified memory ordering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@discardableResult
func logicalXor(
    _ operand: Bool,
    ordering: AtomicUpdateOrdering
) -> (oldValue: Bool, newValue: Bool)
```

Available when `Value` is `Bool`.

## Parameters 

`operand`  

A boolean value.

`ordering`  

The memory ordering to apply on this operation.

## Return Value

A tuple with the old value before the operation a the new value after the operation.

