

- Combine
- Publishers
- Publishers.Scan
-  upstream 

Instance Property

# upstream

The publisher that this publisher receives elements from.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let upstream: Upstream
```

## See Also

### Inspecting Publisher Properties

let initialResult: Output

The previous result returned by the `nextPartialResult` closure.

let nextPartialResult: (Output, Upstream.Output) -> Output

An error-throwing closure that takes as its arguments the previous value returned by the closure and the next element emitted from the upstream publisher.

