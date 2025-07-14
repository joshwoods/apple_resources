

- Combine
- Publishers
- Publishers.Reduce
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

The initial value provided on the first invocation of the closure.

let nextPartialResult: (Output, Upstream.Output) -> Output

A closure that takes the previously-accumulated value and the next element from the upstream publisher to produce a new value.

