

- Combine
- Publishers
- Publishers.TryReduce
-  nextPartialResult 

Instance Property

# nextPartialResult

An error-throwing closure that takes the previously-accumulated value and the next element from the upstream to produce a new value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let nextPartialResult: (Output, Upstream.Output) throws -> Output
```

## Discussion

If this closure throws an error, the publisher fails and passes the error to its subscriber.

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let initial: Output

The initial value provided on the first-use of the closure.

