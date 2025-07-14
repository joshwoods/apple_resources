

- Combine
- Publishers
- Publishers.Catch
-  upstream 

Instance Property

# upstream

The publisher from which this publisher receives its elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let upstream: Upstream
```

## See Also

### Inspecting Publisher Properties

let handler: (Upstream.Failure) -> NewPublisher

A closure that accepts the upstream failure as input and returns a publisher to replace the upstream publisher.

