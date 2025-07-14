

- Synchronization
- Atomic
-  exchange(\_:ordering:) 

Instance Method

# exchange(\_:ordering:)

Atomically sets the current value to `desired` and returns the original value, applying the specified memory ordering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func exchange(
    _ desired: consuming Value,
    ordering: AtomicUpdateOrdering
) -> Value
```

Available when `Value` conforms to `AtomicRepresentable` and `Value.AtomicRepresentation` is `_Atomic64BitStorage`.

## Parameters 

`desired`  

The desired new value.

`ordering`  

The memory ordering to apply on this operation.

## Return Value

The original value.

