

- Combine
- Publishers
- Publishers.TryCatch
-  handler 

Instance Property

# handler

A closure that accepts the upstream failure as input and either returns a publisher to replace the upstream publisher or throws an error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let handler: (Upstream.Failure) throws -> NewPublisher
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives its elements.

