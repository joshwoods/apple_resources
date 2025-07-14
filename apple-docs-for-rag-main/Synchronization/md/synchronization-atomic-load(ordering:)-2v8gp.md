

- Synchronization
- Atomic
-  load(ordering:) 

Instance Method

# load(ordering:)

Atomically loads and returns the current value, applying the specified memory ordering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func load(ordering: AtomicLoadOrdering) -> Value
```

Available when `Value` conforms to `AtomicRepresentable` and `Value.AtomicRepresentation` is `_Atomic8BitStorage`.

## Parameters 

`ordering`  

The memory ordering to apply on this operation.

## Return Value

The current value.

