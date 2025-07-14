

- Synchronization
- AtomicStoreOrdering
-  sequentiallyConsistent 

Type Property

# sequentiallyConsistent

A sequentially consistent store performs a releasing store and also guarantees that it and all other sequentially consistent atomic operations (loads, stores, updates) appear to be executed in a single, total sequential ordering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var sequentiallyConsistent: AtomicStoreOrdering { get }
```

## Discussion

This value corresponds to `std::memory_order_seq_cst` in C++.

