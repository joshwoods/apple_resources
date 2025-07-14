

- Combine
- Publishers
- Publishers.TryReduce
-  upstream 

Instance Property

# upstream

The publisher from which this publisher receives elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let upstream: Upstream
```

## See Also

### Inspecting Publisher Properties

let initial: Output

The initial value provided on the first-use of the closure.

let nextPartialResult: (Output, Upstream.Output) throws -> Output

An error-throwing closure that takes the previously-accumulated value and the next element from the upstream to produce a new value.

