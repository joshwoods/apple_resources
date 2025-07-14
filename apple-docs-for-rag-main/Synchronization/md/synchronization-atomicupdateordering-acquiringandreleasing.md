

- Synchronization
- AtomicUpdateOrdering
-  acquiringAndReleasing 

Type Property

# acquiringAndReleasing

An acquiring-and-releasing operation is a combination of `.acquiring` and `.releasing` operation on the same variable.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var acquiringAndReleasing: AtomicUpdateOrdering { get }
```

## Discussion

This value corresponds to `std::memory_order_acq_rel` in C++.

