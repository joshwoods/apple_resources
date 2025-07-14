

- Combine
- Publishers
- Publishers.CompactMap
-  transform 

Instance Property

# transform

A closure that receives values from the upstream publisher and returns optional values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let transform: (Upstream.Output) -> Output?
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

