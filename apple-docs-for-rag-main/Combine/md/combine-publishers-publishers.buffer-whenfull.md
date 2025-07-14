

- Combine
- Publishers
- Publishers.Buffer
-  whenFull 

Instance Property

# whenFull

The action to take when the buffer becomes full.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let whenFull: Publishers.BufferingStrategy.Failure>
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let size: Int

The maximum number of elements to store.

let prefetch: Publishers.PrefetchStrategy

The strategy for initially populating the buffer.

