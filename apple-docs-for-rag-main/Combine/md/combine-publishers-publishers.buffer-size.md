

- Combine
- Publishers
- Publishers.Buffer
-  size 

Instance Property

# size

The maximum number of elements to store.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let size: Int
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let prefetch: Publishers.PrefetchStrategy

The strategy for initially populating the buffer.

let whenFull: Publishers.BufferingStrategy&lt;Publishers.Buffer&lt;Upstream>.Failure>

The action to take when the buffer becomes full.

