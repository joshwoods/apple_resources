

- Combine
- Publishers
- Publishers.TryFilter
-  isIncluded 

Instance Property

# isIncluded

An error-throwing closure that indicates whether this filter should republish an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let isIncluded: (Upstream.Output) throws -> Bool
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

