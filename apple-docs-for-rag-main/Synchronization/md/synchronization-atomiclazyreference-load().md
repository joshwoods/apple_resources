

- Synchronization
- AtomicLazyReference
-  load() 

Instance Method

# load()

Atomically loads and returns the current value of this reference.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func load() -> Instance?
```

## Return Value

A value of `Instance` if the lazy reference was written to, or `nil` if it has not been written to yet.

## Discussion

Note

The load operation is performed with the memory ordering `AtomicLoadOrdering.acquiring`.

