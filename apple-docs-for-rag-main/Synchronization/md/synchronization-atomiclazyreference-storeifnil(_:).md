

- Synchronization
- AtomicLazyReference
-  storeIfNil(\_:) 

Instance Method

# storeIfNil(\_:)

Atomically initializes this reference if its current value is nil, then returns the initialized value. If this reference is already initialized, then `storeIfNil(_:)` discards its supplied argument and returns the current value without updating it.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func storeIfNil(_ desired: consuming Instance) -> Instance
```

## Parameters 

`desired`  

A value of `Instance` that we will attempt to store if the lazy reference is currently nil.

## Return Value

The value of `Instance` that was successfully stored within the lazy reference. This may or may not be the same value of `Instance` that was passed to this function.

## Discussion

The following example demonstrates how this can be used to implement a thread-safe lazily initialized reference:

```
class Image {
  let _histogram = AtomicLazyReference()

  // This is safe to call concurrently from multiple threads.
  var atomicLazyHistogram: Histogram {
    if let histogram = _histogram.load() { return histogram }
    // Note that code here may run concurrently on
    // multiple threads, but only one of them will get to
    // succeed setting the reference.
    let histogram = ...
    return _histogram.storeIfNil(histogram)
  }
}
```

Note

This operation uses acquiring-and-releasing memory ordering.

