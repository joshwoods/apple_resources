

- Synchronization
- AtomicStoreOrdering
-  relaxed 

Type Property

# relaxed

Guarantees the atomicity of the specific operation on which it is applied, but imposes no ordering constraints on any other variable accesses.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var relaxed: AtomicStoreOrdering { get }
```

## Discussion

This value corresponds to `std::memory_order_relaxed` in C++.

