

- Combine
- Publishers
- Publishers.AllSatisfy
-  predicate 

Instance Property

# predicate

A closure that evaluates each received element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let predicate: (Upstream.Output) -> Bool
```

## Discussion

Return `true` to continue, or `false` to cancel the upstream and finish.

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

