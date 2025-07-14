

- Combine
- Publishers
- Publishers.Reduce
-  nextPartialResult 

Instance Property

# nextPartialResult

A closure that takes the previously-accumulated value and the next element from the upstream publisher to produce a new value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let nextPartialResult: (Output, Upstream.Output) -> Output
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let initial: Output

The initial value provided on the first invocation of the closure.

