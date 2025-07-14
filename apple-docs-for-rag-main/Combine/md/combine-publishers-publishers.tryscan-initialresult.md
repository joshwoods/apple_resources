

- Combine
- Publishers
- Publishers.TryScan
-  initialResult 

Instance Property

# initialResult

The previous result returned by the `nextPartialResult` closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let initialResult: Output
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher that this publisher receives elements from.

let nextPartialResult: (Output, Upstream.Output) throws -> Output

An error-throwing closure that takes as its arguments the previous value returned by the closure and the next element emitted from the upstream publisher.

