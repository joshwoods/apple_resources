

- Combine
- Publishers
- Publishers.Collect
-  buffer(size:prefetch:whenFull:) 

Instance Method

# buffer(size:prefetch:whenFull:)

Buffers elements received from an upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func buffer(
    size: Int,
    prefetch: Publishers.PrefetchStrategy,
    whenFull: Publishers.BufferingStrategy
) -> Publishers.Buffer
```

## Parameters 

`size`  

The maximum number of elements to store.

`prefetch`  

The strategy to initially populate the buffer.

`whenFull`  

The action to take when the buffer becomes full.

## Return Value

A publisher that buffers elements received from an upstream publisher.

## Discussion

Use buffer(size:prefetch:whenFull:) to collect a specific number of elements from an upstream publisher before republishing them to the downstream subscriber according to the Publishers.BufferingStrategy and Publishers.PrefetchStrategy strategy you specify.

If the publisher completes before reaching the `size` threshold, it buffers the elements and publishes them downstream prior to completion.

