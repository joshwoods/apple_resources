

- Combine
- Publishers
- Publishers.TryLastWhere
-  predicate 

Instance Property

# predicate

The error-throwing closure that determines whether to publish an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let predicate: (Publishers.TryLastWhere.Output) throws -> Bool
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

