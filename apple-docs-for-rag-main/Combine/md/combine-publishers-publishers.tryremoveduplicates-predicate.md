

- Combine
- Publishers
- Publishers.TryRemoveDuplicates
-  predicate 

Instance Property

# predicate

An error-throwing closure to evaluate whether two elements are equivalent, for purposes of filtering.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let predicate: (Publishers.TryRemoveDuplicates.Output, Publishers.TryRemoveDuplicates.Output) throws -> Bool
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

