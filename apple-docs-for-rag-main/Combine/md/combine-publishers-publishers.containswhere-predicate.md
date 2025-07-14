

- Combine
- Publishers
- Publishers.ContainsWhere
-  predicate 

Instance Property

# predicate

The closure that determines whether the publisher should consider an element as a match.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let predicate: (Upstream.Output) -> Bool
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

