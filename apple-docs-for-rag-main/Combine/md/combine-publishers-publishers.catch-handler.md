

- Combine
- Publishers
- Publishers.Catch
-  handler 

Instance Property

# handler

A closure that accepts the upstream failure as input and returns a publisher to replace the upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let handler: (Upstream.Failure) -> NewPublisher
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives its elements.

